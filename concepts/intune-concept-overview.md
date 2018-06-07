# <a name="intune-devices-and-apps-api-overview"></a>Überblick über Intune-Geräte und die Apps-API

Mit Microsoft Intune können Unternehmen Geräte und Apps verwalten. Sie können mit der Intune-API in Microsoft Graph Geräte und Apps verwalten sowie Intune mit en von Ihnen bevorzugten Tools konfigurieren. 

Wenn Sie ein ISV sind, können Sie mit der Intune-API auch Kundenmandanten verwalten.

## <a name="why-integrate-with-intune"></a>Gründe für die Integration mit Intune

Sie können die Intune-API in Microsoft Graph verwenden, um auf Intune Geräte- und -Anwendungsinformationen zuzugreifen, Geräte und Apps zu verwalten und Intune zu automatisieren.

### <a name="manage-devices"></a>Verwalten von Geräten

Die Intune-API bietet Ihnen die folgenden Möglichkeiten:

- Definieren und Durchsetzen von [Geräte-Compliance](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md)-Richtlinien, wie z. B. Komplexität und Lebensdauer von Kennwörtern, Verschlüsselung, Bedrohungsschutzstufen usw.  (Welche Richtlinien unterstützt werden, hängt vom Betriebssystem und der Version ab.)
- [Schützen von Unternehmensdaten](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md), und zwar unabhängig davon, ob die Geräteplattform Windows, Android, Mac oder iOS ist.
- Erstellen und Bereitstellen von [Gerätekonfigurationsrichtlinien](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md), einschließlich Betriebssystemplattform/-versionierung, Domänenmitgliedschaft und Verwaltung von Konfigurationseinstellungen.
- Erstellen und Bereitstellen der [Zugriffssteuerungsrichtlinien](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md) für Geräte, einschließlich eingeschränktem Download, Zugriff auf Netzwerkgeräte und Dateiübertragung.
- Durchführen von [Remote-Aktionen](../api-reference/v1.0/resources/intune_devices_manageddevice.md), wie z. B. das Lokalisieren von Geräten, Ändern von Kennwörtern und Löschen von Gerätedaten.

### <a name="manage-apps"></a>Verwalten von Apps 

Mit der Intune-API können Sie die folgenden Aufgaben für die App-Verwaltung ausführen:

- Bereitstellen von [Apps auf Geräten](../api-reference/v1.0/resources/intune_apps_mobileapp.md) oder das Bereitstellen von Apps verhindern.
- Verwalten des Zugriffs auf [e-Books](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md) und zugehörige Dienste.
- Definieren und Bereitstellen von App-Konfigurationseinstellungen, Einstellungen für den App-Schutz und Verwendungsrichtlinien für Apps.

### <a name="automate-intune"></a>Automatisieren von Intune

Die Intune-API bietet die folgenden Automatisierungsfunktionen:

- Definieren und Zuweisen von [rollenbasierten](../api-reference/v1.0/resources/intune_rbac_conceptual.md) Zugriffssteuerungen.
- Prüfen der Compliance, Verwendung und des Zugriffs sowie entsprechende Berichterstattung.
- Verwalten von [Telekommunikationsausgaben](../api-reference/v1.0/resources/intune_tem_conceptual.md).


## <a name="next-steps"></a>Nächste Schritte

- [Verwenden von Azure AD für den Zugriff auf die Intune-API](https://docs.microsoft.com/intune/intune-graph-apis).
- Informationen zum Ausführen allgemeiner Aufgaben mithilfe der [PowerShell-Intune-Beispiele](https://github.com/microsoftgraph/powershell-intune-samples).
- Informationen zum [Verwenden der Intune-REST-API](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/intune_graph_overview).
- Informationen zu Neuerungen in der Intune-API finden Sie im [Changelog](changelog.md).
- In den [Beispielen](https://developer.microsoft.com/de-DE/graph/graph/examples) finden Sie weitere Ideen für die Verwendung von Microsoft Graph.
