---
title: Integrieren von Sicherheits-API-Warnungen in Microsoft Graph in SIEM (Security Information & Event Management)
description: Mit der Sicherheits-API von Microsoft Graph können Sicherheitshinweise als allen Microsoft-Sicherheitsprodukten (als Microsoft Graph-Sicherheitsanbieter bezeichnet) über einen einzigen REST-Endpunkt verwaltet werden. Einige Organisationen erfassen vielleicht schon Azure-spezifische Protokolldaten über Azure Monitor in SIEM-Lösungen. Zur Vereinfachung der Integration können die über die Sicherheits-API in Microsoft Graph verfügbaren Sicherheitshinweise auch über Azure Monitor vom Kunden für das Abonnement bereitgestellt werden. Wenn Ihre Organisation die Azure Monitor-Integration mit Ihrer SIEM-Lösung bereits konfiguriert hat, können Sie jetzt ganz einfach die Sicherheitswarnungen Ihrer Organisation den vorhandenen Daten hinzufügen, die über Azure Monitor verfügbar sind.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 10adbecb5f82556e5acc2301fc226ae6884e142b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/20/2019
ms.locfileid: "30693687"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integrieren von Sicherheits-API-Warnungen in Microsoft Graph in SIEM (Security Information & Event Management)

Mit der Sicherheits-API von Microsoft Graph können Sicherheitshinweise als allen Microsoft-Sicherheitsprodukten (als Microsoft Graph-Sicherheitsanbieter bezeichnet) über einen einzigen REST-Endpunkt verwaltet werden. Einige Organisationen erfassen vielleicht schon Azure-spezifische Protokolldaten über Azure Monitor in SIEM-Lösungen. Zur Vereinfachung der Integration können die über die Sicherheits-API in Microsoft Graph verfügbaren Sicherheitshinweise auch über Azure Monitor vom Kunden für das Abonnement bereitgestellt werden. Wenn Ihre Organisation die Azure Monitor-Integration mit Ihrer SIEM-Lösung bereits konfiguriert hat, können Sie jetzt ganz einfach die Sicherheitswarnungen Ihrer Organisation den vorhandenen Daten hinzufügen, die über Azure Monitor verfügbar sind.

Warnungen der folgenden Sicherheitsanbieter sind über die SIEM-Integration verfügbar:

- [Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(Vorschau)**
- [Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) **(Vorschau)**
- [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(Vorschau)**

Azure Monitor unterstützt Connectors mit mehreren SIEM-Produkten. Eine Liste der unterstützten SIEM-Produkte finden Sie unter [Senden von Überwachungsdaten an ein Ereignis-Hub](https://docs.microsoft.com/de-DE/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Die Integration der Sicherheits-API in Microsoft Graph-API ist derzeit für [Splunk](https://splunkbase.splunk.com/) und [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) verfügbar.

Informationen zur Integration der Sicherheits-API in Microsoft Graph für spezifische SIEM-Lösungen finden Sie unter:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
