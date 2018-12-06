---
title: Überblick über Intune-Geräte und die Apps-API
description: 'Mit Microsoft Intune können Unternehmen Geräte und Apps verwalten. Sie können mit der Intune-API in Microsoft Graph Geräte und Apps verwalten sowie Intune mit en von Ihnen bevorzugten Tools konfigurieren. '
ms.openlocfilehash: fced71d317aa5f2aebfd2c44237ea9087a6be4f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092284"
---
# <a name="intune-devices-and-apps-api-overview"></a>Überblick über Intune-Geräte und die Apps-API

Mit Microsoft Intune können Unternehmen Geräte und Apps verwalten. Sie können mit der Intune-API in Microsoft Graph Geräte und Apps verwalten sowie Intune mit en von Ihnen bevorzugten Tools konfigurieren. 

Wenn Sie ein ISV sind, können Sie mit der Intune-API auch Kundenmandanten verwalten.

## <a name="why-integrate-with-intune"></a>Gründe für die Integration mit Intune

Sie können die Intune-API in Microsoft Graph verwenden, um auf Intune Geräte- und -Anwendungsinformationen zuzugreifen, Geräte und Apps zu verwalten und Intune zu automatisieren.

### <a name="manage-devices"></a>Verwalten von Geräten

Die Intune-API bietet Ihnen die folgenden Möglichkeiten:

- Definieren und Durchsetzen von [Geräte-Compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)-Richtlinien, wie z. B. Komplexität und Lebensdauer von Kennwörtern, Verschlüsselung, Bedrohungsschutzstufen usw.  (Welche Richtlinien unterstützt werden, hängt vom Betriebssystem und der Version ab.)
- [Schützen von Unternehmensdaten](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), und zwar unabhängig davon, ob die Geräteplattform Windows, Android, Mac oder iOS ist.
- Erstellen und Bereitstellen von [Gerätekonfigurationsrichtlinien](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), einschließlich Betriebssystemplattform/-versionierung, Domänenmitgliedschaft und Verwaltung von Konfigurationseinstellungen.
- Erstellen und Bereitstellen der [Zugriffssteuerungsrichtlinien](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) für Geräte, einschließlich eingeschränktem Download, Zugriff auf Netzwerkgeräte und Dateiübertragung.
- Durchführen von [Remote-Aktionen](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), wie z. B. das Lokalisieren von Geräten, Ändern von Kennwörtern und Löschen von Gerätedaten.

### <a name="manage-apps"></a>Verwalten von Apps 

Mit der Intune-API können Sie die folgenden Aufgaben für die App-Verwaltung ausführen:

- Bereitstellen von [Apps auf Geräten](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) oder das Bereitstellen von Apps verhindern.
- Verwalten des Zugriffs auf [e-Books](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) und zugehörige Dienste.
- Definieren und Bereitstellen von App-Konfigurationseinstellungen, Einstellungen für den App-Schutz und Verwendungsrichtlinien für Apps.

### <a name="automate-intune"></a>Automatisieren von Intune

Die Intune-API bietet die folgenden Automatisierungsfunktionen:

- Definieren und Zuweisen von [rollenbasierten](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) Zugriffssteuerungen.
- Prüfen der Compliance, Verwendung und des Zugriffs sowie entsprechende Berichterstattung.
- Verwalten von [Telekommunikationsausgaben](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Intune-API in Microsoft Graph v1.0](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [Intune-API in Microsoft Graph, Betaversion](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

- [Verwenden von Azure AD für den Zugriff auf die Intune-API](https://docs.microsoft.com/intune/intune-graph-apis).
- Informationen zum Ausführen allgemeiner Aufgaben mithilfe der [PowerShell-Intune-Beispiele](https://github.com/microsoftgraph/powershell-intune-samples).
- Informationen zum [Verwenden der Intune-REST-API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).
- Informationen zu Neuerungen in der Intune-API finden Sie im [Changelog](changelog.md).
- In den [Beispielen](https://developer.microsoft.com/graph/graph/examples) finden Sie weitere Ideen für die Verwendung von Microsoft Graph.
