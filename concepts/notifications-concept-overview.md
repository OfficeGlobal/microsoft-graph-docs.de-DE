# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Verwendung der Benachrichtigungs-API in Microsoft Graph, um eine benutzerzentrierte Benachrichtigung zu ermöglichen 

Benachrichtigungen sind der effektivste Weg, um Ihre Benutzer wieder zu aktivieren. Sie können die Aufmerksamkeit Ihrer Benutzer auf sich ziehen und sie zu Ihrer Anwendung zurückbringen. In einer Umgebung mit mehreren Geräten können Ihre Benutzer von überall auf Ihre Anwendungen und Dienste zugreifen und zwar über verschiedene Plattformen und Geräte, auf denen Ihre Apps verfügbar sind. 

Ihre Benachrichtigungsszenarien sollten „benutzerzentriert“ gestaltet sein, wobei das Hauptziel darin besteht, den Benutzer zu benachrichtigen, wo immer er sich gerade befindet. Bestehende Benachrichtigungslösungen, die von den wichtigsten Plattformen angeboten werden, eignen sich hervorragend zur Ausrichtung auf Geräte. Microsoft Graph-Benachrichtigungen verbessern dies, indem sie es Ihnen ermöglichen, Benutzer gezielt anzusprechen. Microsoft Graph-Benachrichtigungen übernehmen komplexe Aufgaben wie die Zuordnung zwischen Benutzern und Endpunkten, die Synchronisierung des Benachrichtigungsstatus zwischen den verschiedenen Endpunkten der Benutzer und vieles mehr. 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Vorteile der Integration von Microsoft Graph-Benachrichtigungen:
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>Benachrichtigung eines Benutzers über verschiedene Endpunkte hinweg
Als Teil von Microsoft Graph ermöglicht Ihnen die Benachrichtigungs-API, eine Benachrichtigung an ein Microsoft-Konto oder ein Arbeits- oder Schulkonto (Azure AD) zu senden. Die Plattform verteilt diese Benachrichtigung an alle Endpunkte des Benutzers, einschließlich Windows UWP, Android und iOS. 

### <a name="manage-notifications-across-endpoints"></a>Verwaltung von Benachrichtigungen über Endpunkte hinweg
Die Microsoft Graph-Benachrichtigungs-API ermöglicht es Ihnen, den Status einer Benachrichtigung zu aktualisieren und diesen Status über alle Endpunkte hinweg zu synchronisieren. Wenn ein Benutzer beispielsweise auf eine Benachrichtigung auf einem Gerät reagiert, können Sie den Status dieser Benachrichtigung aktualisieren (z. B. als gelesen oder abgelehnt markieren). Die gleiche Zustandsänderung wird auf alle anderen Endpunkte verteilt. Die Microsoft Graph-Benachrichtigungs-API verfolgt den Status der Benachrichtigungen Ihrer Benutzer auf zentralisierte Weise und macht es Ihnen leicht, sicherzustellen, dass Ihre Benachrichtigungen nur einmal bearbeitet und überall abgeglichen werden.

### <a name="retrieve-notification-history"></a>Benachrichtigungsverlauf abrufen
Sie können die Benachrichtigungs-API verwenden, um die Benachrichtigungshistorie basierend auf einer von Ihnen definierten Ablaufzeit (bis zu 30 Tage) abzurufen. Benachrichtigungen, die als gelesen oder abgewiesen markiert wurden, sind weiterhin aus der Historie abrufbar, sodass In-App-Ansichten des Benachrichtigungsverlaufs und anderer Szenarien möglich sind. 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Integration mit der Benachrichtigungs-API in Microsoft Graph

Sie können Ihre Anwendungen mit Microsoft Graph-Benachrichtigungen in wenigen einfachen Schritten integrieren - verbinden Sie Ihre Anwendung über das Windows Dev Center, verwenden Sie die Methode [Benachrichtigung erstellen](../api-reference/beta/api/projectrome_notification_post.md), um Benachrichtigungen zu veröffentlichen und verwenden Sie das Project-Rome-SDK, um Benachrichtigungen auf Ihren App-Clients zu empfangen und zu verwalten.  

Weitere Informationen zur Verteilung von Benutzerbenachrichtigungen über Microsoft Graph finden Sie in der [Benachrichtigungs-API-Referenz](../api-reference/beta/resources/notifications-api-overview.md).
 
Weitere Informationen zum Empfangen und Verwalten von Benachrichtigungen durch die Integration mit dem Project-ROM-SDK finden Sie in der [Project-ROM-SDK-Dokumentation](https://docs.microsoft.com/en-us/windows/project-rome/) 

## <a name="see-also"></a>Siehe auch

- [Geräteübergreifende Oberflächen in Microsoft Graph](cross-device-concept-overview.md)
- [Projekt ROM Developer-Center](http://aka.ms/projectrome)
