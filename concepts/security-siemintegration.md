---
title: Integrieren von Sicherheits-API-Warnungen in Microsoft Graph in SIEM (Security Information & Event Management)
description: Mit der Sicherheits-API von Microsoft Graph können Sicherheitshinweise als allen Microsoft-Sicherheitsprodukten (als Microsoft Graph-Sicherheitsanbieter bezeichnet) über einen einzigen REST-Endpunkt verwaltet werden. Einige Organisationen erfassen vielleicht schon Azure-spezifische Protokolldaten über Azure Monitor in SIEM-Lösungen. Zur Vereinfachung der Integration können die über die Sicherheits-API in Microsoft Graph verfügbaren Sicherheitshinweise auch über Azure Monitor vom Kunden für das Abonnement bereitgestellt werden. Wenn Ihre Organisation die Azure Monitor-Integration mit Ihrer SIEM-Lösung bereits konfiguriert hat, können Sie jetzt ganz einfach die Sicherheitswarnungen Ihrer Organisation den vorhandenen Daten hinzufügen, die über Azure Monitor verfügbar sind.
ms.openlocfilehash: ca2952163ab8894cae4c22f726b45b1be94a8b1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092251"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integrieren von Sicherheits-API-Warnungen in Microsoft Graph in SIEM (Security Information & Event Management)

Mit der Sicherheits-API von Microsoft Graph können Sicherheitshinweise als allen Microsoft-Sicherheitsprodukten (als Microsoft Graph-Sicherheitsanbieter bezeichnet) über einen einzigen REST-Endpunkt verwaltet werden. Einige Organisationen erfassen vielleicht schon Azure-spezifische Protokolldaten über Azure Monitor in SIEM-Lösungen. Zur Vereinfachung der Integration können die über die Sicherheits-API in Microsoft Graph verfügbaren Sicherheitshinweise auch über Azure Monitor vom Kunden für das Abonnement bereitgestellt werden. Wenn Ihre Organisation die Azure Monitor-Integration mit Ihrer SIEM-Lösung bereits konfiguriert hat, können Sie jetzt ganz einfach die Sicherheitswarnungen Ihrer Organisation den vorhandenen Daten hinzufügen, die über Azure Monitor verfügbar sind.

Azure Monitor unterstützt Connectors mit mehreren SIEM-Produkten. Eine Liste der unterstützten SIEM-Produkte finden Sie unter [Senden von Überwachungsdaten an ein Ereignis-Hub](https://docs.microsoft.com/de-DE/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Die Integration der Sicherheits-API in Microsoft Graph-API ist derzeit für [Splunk](https://splunkbase.splunk.com/) und [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) verfügbar.

Informationen zur Integration der Sicherheits-API in Microsoft Graph für spezifische SIEM-Lösungen finden Sie unter:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
