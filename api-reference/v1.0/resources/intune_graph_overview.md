# <a name="working-with-intune-in-microsoft-graph"></a>Arbeiten mit Intune in Microsoft Graph  

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/de-DE/cloud-platform/microsoft-intune-pricing) ist.

Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.  

In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/de-DE/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt. 

## <a name="using-the-intune-graph-api"></a>Verwenden der Graph-API für Intune

Intune stellt Daten auf die gleiche Weise für die Microsoft Graph-API bereit, wie es auch andere Clouddienste tun, mit detaillierten Informationen zu Entitäten und Möglichkeiten zur Beziehungsnavigation.  Mithilfe der Microsoft Graph-API können Sie Informationen aus anderen Diensten und aus Intune miteinander kombinieren und so funktionsreiche, dienstübergreifende Anwendungen für IT-Experten oder Endbenutzer erstellen.     

Das Beispiel unten demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist: 

1. Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a>Verwenden von Berechtigungsbereichen

Die Microsoft Graph-API steuert den Zugriff auf Ressourcen mithilfe von Berechtigungsbereichen. Als Entwickler müssen Sie die Berechtigungsbereiche angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen. In der Regel geben Sie die benötigten Berechtigungsbereiche im Azure Active Directory-Portal an. Weitere Informationen finden Sie im Artikel zu den Themen [Microsoft Graph-Berechtigungsbereiche](https://developer.microsoft.com/de-DE/graph/docs/authorization/permission_scopes) und [Intune-Berechtigungsbereiche](https://developer.microsoft.com/de-DE/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).

