# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integrieren von Microsoft Graph Sicherheits-API-Warnungen in einer SIEM

Die Microsoft Graph-Security-API ermöglicht die Verwaltung von Sicherheitshinweisen von allen Microsoft Security-Produkten, bekannt als Microsoft Graph-Sicherheitsanbieter, über einen einzelnen REST-Endpunkt. Einige Organisationen haben möglicherweise bereits Azure-spezifische Protokolldaten über Azure Monitor in SIEM Lösungen aufgenommen. Zur Vereinfachung der Integration können über die Sicherheit-API von Microsoft Graph verfügbare Sicherheitswarnungen auch durch den Kunden auf ihr Abonnement über Azure Monitor bereitgestellt werden. Wenn Ihre Organisation bereits die Azure Monitor Integration mit Ihrer SIEM-Lösung konfiguriert hat, können Sie jetzt problemlos Sicherheitshinweise Ihrer Organisation zusätzlich zu den vorhandenen Daten über Azure Monitor streamen.

Azure Monitor unterstützt Connectors für mehrere SIEM-Produkte. Eine Liste der unterstützten SIEM-Produkte finden Sie unter [Überwachungsdaten an einen Ereignis-Hub senden](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Die Microsoft Graph-Sicherheits-API-Integration ist derzeit für [Splunk](https://splunkbase.splunk.com/) und [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)verfügbar.

Informationen zur Integration der Microsoft Graph-Sicherheits-API für bestimmte SIEM-Lösungen finden Sie unter:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
