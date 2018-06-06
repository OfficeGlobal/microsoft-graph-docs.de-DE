# <a name="overview-of-security-in-microsoft-graph-preview"></a>Übersicht über die Sicherheit in Microsoft Graph (Vorschau) 

Sie können Microsoft Graph für die Verbindung mit Intelligent Security Graph verwenden, um Ressourcen von Microsoft und von Sicherheitspartnern zu nutzen und bessere Lösungen zur Reaktion auf Bedrohungen zu erstellen. Microsoft Graph bietet auch Zugriff auf Benutzer- und Kontorisiken, die vom Identity Protection-Dienst in Azure Active Directory (Azure AD) erkannt werden, sodass Sie Daten zu Kontorisiken in Ihre Sicherheitsanwendungen integrieren können.

## <a name="why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph"></a>Warum sollten Sie die Sicherheits-API verwenden und eine Verbindung mit Microsoft Intelligent Security Graph herstellen?

Intelligent Security Graph ist eine einheitliche Plattform für die Bekämpfung von Cyberthreats. Es ermöglicht Bedrohungsschutz für Microsoft-Produkte und Dienste in Echtzeit und unterstützt ein Ökosystem von integrierten Lösungen.

Die [Sicherheits-API in Microsoft Graph](https://aka.ms/graphsecuritydocs) erleichtert das Herstellen einer Verbindung mit diesen Lösungen in Intelligent Security Graph. Sie ermöglicht es Ihnen, den Wert dieser Lösungen besser zu erkennen und ggf. zu erweitern.

### <a name="unify-and-standardize-alert-management"></a>Vereinheitlichen und Standardisieren der Warnungsverwaltung

Korrelieren Sie Warnungen über Sicherheitslösungen hinweg mit einem gemeinsamen Warnungsschema. Schreiben Sie einmalig Code, um Warnungen aus beliebigen in Microsoft Graph integrierten Sicherheitslösungen zu integrieren, und halten Sie Warnungsstatus und Aufgaben für alle Lösungen synchronisiert. Sie können Warnungen auch zu SIEM-Lösungen (Security Information and Event Management) wie Splunk und IBM QRadar über [Azure Monitor](https://docs.microsoft.com/de-DE/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) streamen.

### <a name="federated-security-aggregation-service"></a>Dienst zur Aggregation von Verbundsicherheit

Verwenden Sie die Sicherheits-API als Dienst zur Aggregation von Verbundsicherheit, um Abfragen an alle integrierten Sicherheitsanbieter zu übermitteln und zusammengefasste Antworten zu erhalten.

### <a name="unlock-security-context-to-drive-investigation"></a>Aufheben der Sperrung von Sicherheitskontext zu Untersuchungszwecken

Gewinnen Sie Einblicke in den sicherheitsrelevanten Bestand (z. B. Benutzer, Hosts und Apps), und fügen Sie organisatorischen Kontext von anderen Microsoft Graph-Anbietern (Azure Active Directory, Microsoft Intune, Office 365) hinzu, um Business- und Sicherheitskontexte zusammenzubringen und die Reaktion auf Sicherheitsrisiken zu verbessern.

## <a name="why-use-azure-ad-to-protect-identities-in-your-organization"></a>Warum mithilfe von Azure AD Identitäten in Ihrer Organisation schützen?

Die meisten Sicherheitsverletzungen entstehen dadurch, dass Angreifer die Identität eines Benutzers stehlen. Zudem nutzen Angreifer erschreckend effektiv Sicherheitsrisiken durch Drittanbieter, Password-Spray-Angriffe und ausgeklügelte Phishingangriffe aus. Dies bedeutet, dass Sie alle Benutzerkonten vor diesen Angriffen schützen und proaktiv verhindern müssen, dass manipulierte Identitäten missbraucht werden können.

Azure Active Directory verwendet adaptive Machine Learning-Algorithmen und Heuristiken, um Anomalien zu erkennen, die auf potenziell kompromittierte Konten hinweisen. Mit diesen Daten schützt Identity Protection Ihre Benutzer mit risikobasierten Richtlinien für bedingten Zugriff und generiert Berichte und Benachrichtigungen zu deren Erkennung.

Aktuell bietet Microsoft Graph Kunden mit Azure AD Premium P1 und P2 einfachen Zugriff, um von Identity Protection erkannte Risiken abzufragen und diese Ereignisse in SIEM-Systemen und Sicherheitsanwendungen zu verwenden.

## <a name="next-steps"></a>Nächste Schritte

- [Verwenden der Sicherheits-API](../api-reference/beta/resources/security-api-overview.md)
- [Verwenden der Azure AD Identity Protection-API](../api-reference/beta/resources/identityprotection_root.md)

