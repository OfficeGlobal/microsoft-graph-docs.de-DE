# <a name="microsoft-graph-permission-scopes"></a>Microsoft Graph-Berechtigungsbereiche

Microsoft Graph macht OAuth 2.0-Berechtigungsbereiche verfügbar, die den Zugriff von Apps auf Ressourcen steuern. Als Entwickler bestimmen Sie die Berechtigungsbereiche, die für den Zugriff, den Ihre App benötigt, angemessen sind. (Wenn Sie eine Azure AD-Authentifizierung verwenden, tun Sie dies normalerweise über das Azure Management-Portal Wenn Sie den Azure AD v2.0-Endpunkt verwenden, fordern Sie Genehmigungen dynamisch während der Laufzeit an.

Nach der Anmeldung haben Benutzer oder Administratoren die Möglichkeit, zuzustimmen, dass Ihre App auf Ressourcen mit den konfigurierten Berechtigungsbereichen zugreifen kann. Aus diesem Grund sollten Sie Berechtigungsbereiche auswählen, die die niedrigste von Ihrer App benötigte Berechtigungsstufe bereitstellt. Weitere Details zum Konfigurieren von Berechtigungen für Ihre App und zum Zustimmungsprozess finden Sie unter <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-integrating-applications/" target="_newtab">Integrieren von Apps in Azure Active Directory</a>.

>**Hinweis:** Einige Microsoft Graph-Berechtigungen, wie z. B. solche, die zu Gruppen und Aufgaben gehören, gelten nicht für private Konten.  

##<a name="app-only-vs-delegated-permissions"></a>Nur-App-Berechtigungen verglichen mit delegierten Berechtigungen
Berechtigungsbereiche können entweder nur für die App gelten oder delegiert sein. Nur-App-Bereiche (auch als App-Rollen bezeichnet) gewähren der App den vollen Satz von in dem Bereich enthaltenen Berechtigungen. Nur-App-Bereiche werden in der Regel von Apps verwendet, die als Dienst ausgeführt werden, ohne dass ein angemeldeter Benutzer vorhanden ist. 


Delegierte Berechtigungsbereiche gelten für Apps, die im Namen eines Benutzers handeln. Diese Bereiche delegieren die Berechtigungen des angemeldeten Benutzers, sodass die App als der Benutzer auftreten kann. Die der App tatsächlich gewährten Berechtigungen ist die Kombination mit den wenigsten Berechtigungen (die Schnittmenge) der vom Berechtigungsbereich gewährten Rechte und der des angemeldeten Benutzers. Wenn z. B. der Berechtigungsbereich delegierte Berechtigungen zum Schreiben aller Verzeichnisobjekte erteilt, der angemeldete Benutzer aber nur über Berechtigungen zum Aktualisieren seines eigenen Benutzerprofils verfügt, kann die App nur das Profil des angemeldeten Benutzers, aber keine anderen Objekte schreiben.

> **Hinweis**: Bei Gruppen unterstützt nur eine Teilmenge der API, die zur Hauptgruppenadministration und -verwaltung gehören, sowohl Nur-App- als auch delegierte Berechtigungen. Alle anderen Mitglieder der Gruppen-API unterstützen nur delegierte Berechtigungen. Beispiele finden Sie unter [Bekannte Probleme](../overview/release_notes.md#groups).

## <a name="full-and-basic-profiles-for-users-and-groups"></a>Vollständige und einfache Profile für Benutzer und Gruppen

Das vollständige Profil (oder das Profil) eines Benutzers oder einer Gruppe umfasst alle deklarierten Eigenschaften der Entität. Da das Profil möglicherweise vertrauliche Informationen oder personenbezogene Informationen (Personally Identifiable Information, PII) enthält, schränken mehrere Bereiche den App-Zugriff auf eine begrenzte Gruppe von Eigenschaften ein, die als einfaches Profil bezeichnet werden. Für Benutzer umfasst das einfache Profil lediglich folgende Eigenschaften: 

- Anzeigename
- Vor- und Nachname
- Fotopapier
- E-Mail-Adresse

Für Gruppen enthält das einfache Profil nur den Anzeigenamen. 

<!---    <a name="msg_perm_details"> </a>  -->

## <a name="permission-scope-details"></a>Details zu Berechtigungsbereichen

Sie müssen Ihre App konfigurieren, um die notwendigen Ressourcen für den Zugriff auf Microsoft Graph-Ressourcen zu erhalten. Die Berechtigungen gelten für einzelne Ressourcen und umfassen Lese-, Schreibzugriff oder beides. 

In den folgenden Tabellen sind die Microsoft Graph-Berechtigungsbereiche aufgeführt, und es wird der von jeder Berechtigung gewährte Zugriff erläutert. 

- In der Spalte **Bereich** ist der Bereichsname enhalten. Bereichsnamen weisen die Form „resource.operation.constraint“ auf, zum Beispiel „Group.ReadWrite.All“. Bei der Einschränkung „Alles“ wird der App vom Bereich die Möglichkeit gewährt, die Operation (ReadWrite) für alle angegebenen Ressourcen (Gruppe) im Verzeichnis auszuführen. Andernfalls lässt der Bereich die Operation nur in dem Profil des angemeldeten Benutzers zu. Bereiche gewähren möglicherweise eingeschränkte Privilegien für den festgelegten Vorgang. Weitere Details finden Sie in der Spalte **Beschreibung**.
- In der Spalte **Berechtigung** wird gezeigt, wie der Bereich im Azure-Portal angezeigt wird. 
- Die Spalte **Beschreibung** beschreibt den vollständigen Satz von Berechtigungen, die von dem Bereich gewährt werden. Bei delegierten Bereichen ist der der App tatsächlich gewährte Zugriff die Kombination mit den wenigsten Berechtigungen (die Schnittmenge) der vom Bereich gewährten Rechte und der des angemeldeten Benutzers. 
- Die Bereiche werden danach gruppiert, ob die Berechtigungen die Zustimmung eines Administrators erfordern.

  > **Hinweis**: Unter [Bekannte Probleme](../overview/release_notes.md) finden Sie weitere Informationen zu Einschränkungen von Berechtigungsbereichen für `v1.0` und `beta`.
  
###<a name="permissions-requiring-administrators-consent"></a>Berechtigungen, die die Zustimmung des Administrators erfordern

|   **Bereich**                  |  **Berechtigung**                          |  **Beschreibung** |
|:-----------------------------|:-----------------------------------------|:-----------------|
| _Directory.AccessAsUser.All_   |     Als der angemeldete Benutzer auf das Verzeichnis zugreifen  | Die App kann den gleichen Zugriff auf Informationen im Verzeichnis wie der angemeldete Benutzer haben.|
| _Directory.Read.All_           |     Verzeichnisdaten lesen                     | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation zu lesen, z. B. Benutzer, Gruppen und Apps. |
| _Directory.ReadWrite.All_      |     Schreib-/Lesezugriff auf Verzeichnisdaten           | Die App kann Daten im Verzeichnis Ihrer Organisation lesen und schreiben, z. B. Benutzer und Gruppen.  Ermöglicht nicht das Löschen eines Benutzers oder einer Gruppe. Die App kann nicht Benutzer oder Gruppen löschen oder Benutzerkennwörter zurücksetzen. |
| _Group.Read.All_ |    Lesezugriff auf alle Gruppen | Die App kann Gruppen aufführen und deren Eigenschaften sowie alle Gruppenmitgliedschaften im Namen des angemeldeten Benutzers lesen.  Die App kann außerdem, den Kalender, Unterhaltungen, Dateien und andere Gruppeninhalte für alle Gruppen, auf die der Benutzer zugreifen kann, lesen. |
| _Group.ReadWrite.All_ |    Schreib-/Lesezugriff auf alle Gruppen| Die App kann Gruppen erstellen und alle Gruppeneigenschaften und -mitgliedschaften im Namen des angemeldeten Benutzers lesen.  Darüber hinaus können Gruppenbesitzer ihre eigenen Gruppen verwalten, und Gruppenmitglieder können Gruppeninhalte aktualisieren. |
| _User.Read.All_                |     Lesezugriff auf vollständige Profile aller Benutzer           | Identisch mit User.ReadBasic.All, mit der Ausnahme, dass die App das vollständige Profil aller Benutzer in der Organisation lesen kann. Dabei können auch Navigationseigenschaften, z. B. Manager- und direkte Berichte, gelesen werden. Das vollständige Profil enthält alle deklarierten Eigenschaften der **Benutzer**-Entität. Um die Gruppen zu lesen, in denen ein Benutzer Mitglied ist, benötigt die App auch „Group.Read.All“ oder „Group.ReadWrite.All“. |
| _User.ReadWrite.All_           |     Lese- und Schreibzugriff auf vollständige Profile aller Benutzer | Die App kann den vollständigen Satz von Profileigenschaften, Berichte und Vorgesetzte von anderen Benutzern in Ihrer Organisation im Namen des angemeldeten Benutzers lesen und schreiben. |


###<a name="permissions-not-requiring-administrators-consent"></a>Berechtigungen, die keine Zustimmung des Administrators erfordern

|   **Bereich**    |  **Berechtigung**   |  **Beschreibung** |
|:-----------------------------|:-----------------------------------------|:-----------------|
| _Calendars.Read_ |    Benutzerkalender lesen  | Die App kann Ereignisse im Benutzerkalender lesen.|
| _Calendars.Read.Shared_ |    Benutzerkalender und freigegebene Kalender lesen | Die App kann Ereignisse in allen Kalendern lesen, auf die der Benutzer zugreifen kann, einschließlich delegierter und freigegebener Kalender. |
| _Calendars.ReadWrite_ |    Vollzugriff auf Benutzerkalender  | Die App kann Ereignisse im Benutzerkalender erstellen, lesen, aktualisieren und löschen. |
| _Calendars.ReadWrite.Shared_ |    Benutzerkalender und freigegebene Kalender lesen und schreiben | Die App kann Ereignisse in allen Kalendern, für die der Benutzer über Zugriffsberechtigungen verfügt, erstellen, lesen, aktualisieren und löschen. Dies umfasst delegierte und freigegebene Kalender.|
| _Contacts.Read_ |    Benutzerkontakte lesen  | Die App kann Benutzerkontakte lesen. |
| _Contacts.Read.Shared_ |    Benutzerkontakte und freigegebene Kontakte lesen | Die App kann Kontakte lesen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Kontakte des Benutzers und freigegebener Kontakte. |
| _Contacts.ReadWrite_ |    Vollzugriff auf Benutzerkontakte  | Die App kann Benutzerkontakte erstellen, lesen, aktualisieren und löschen. |
| _Contacts.ReadWrite.Shared_ |    Benutzerkontakte und freigegebene Kontakte lesen und schreiben | Die App kann Kontakte lesen aktualisieren und löschen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Kontakte des Benutzers und freigegebener Kontakte.|
| _Files.Read_ |    Lesezugriff auf Benutzerdateien und Dateien, die für den Benutzer freigegeben wurden | Die App kann die Dateien des angemeldeten Benutzers sowie für den Benutzer freigegebene Dateien lesen.| 
| _Files.Read.All_ | Alle Dateien lesen, auf die der Benutzer zugreifen kann | Die App kann alle Dateien lesen, auf die der angemeldete Benutzer zugreifen kann. |
| _Files.Read.Selected_ |    Lesezugriff auf Dateien, die der Benutzer auswählt  | Die App kann Dateien, die der Benutzer auswählt, lesen. Die App hat mehrere Stunden, nachdem der Benutzer eine Datei ausgewählt hat, Zugriff. |
| _Files.ReadWrite_ |   Vollzugriff auf Benutzerdateien und Dateien, die für den Benutzer freigegeben wurden | Die App kann die Dateien des angemeldeten Benutzers sowie für den Benutzer freigegebene Dateien lesen, erstellen, aktualisieren und löschen. |
| _Files.ReadWrite.All_ | Vollzugriff auf alle Dateien, auf die Benutzer zugreifen können | Die App kann alle Dateien lesen, erstellen, aktualisieren und löschen, auf die der angemeldete Benutzer zugreifen kann. |
| _Files.ReadWrite.AppFolder_ | Vollzugriff auf den Anwendungsordner | Die App kann Dateien im Anwendungsordner lesen, erstellen, aktualisieren und löschen. |
| _Files.ReadWrite.Selected_ |    Lese- und Schreibzugriff auf Dateien, die der Benutzer auswählt | Die App kann Dateien, die der Benutzer auswählt, lesen und schreiben. Die App hat mehrere Stunden, nachdem der Benutzer eine Datei ausgewählt hat, Zugriff. |
| _Mail.Read_ |    Benutzer-E-Mails lesen | Die App kann E-Mails in Benutzerpostfächern lesen.  |
| _Mail.Read.Shared_ |    Benutzer-E-Mails und freigegebene E-Mails lesen | Die App kann E-Mails lesen, auf die der Benutzer zugreifen kann, einschließlich der eigenen E-Mails des Benutzers und freigegebener E-Mails. |
| _Mail.ReadWrite_ |    Schreib-/Lesezugriff auf Benutzer-E-Mails | Die App kann E-Mails in Benutzerpostfächern erstellen, lesen, aktualisieren und löschen. Umfasst nicht über die Berechtigung zum Senden von E-Mails.|
| _Mail.ReadWrite.Shared_ |    Benutzer-E-Mails und freigegebene E-Mails lesen und schreiben | Die App kann E-Mails erstellen, lesen, aktualisieren und löschen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen E-Mails des Benutzers und freigegebener E-Mails. Umfasst nicht die Berechtigung zum Senden von E-Mails. |
| _Mail.Send_ |    E-Mails als Benutzer senden | Die App kann E-Mails im Namen der Benutzer in der Organisation senden.  |
| _Mail.Send.Shared_ |    Senden von E-Mails im Auftrag von anderen Benutzern | Die App kann E-Mails, einschließlich der E-Mails im Auftrag von anderen Benutzern, als angemeldeter Benutzer senden. |
| _MailboxSettings.ReadWrite_ |  Benutzerpostfacheinstellungen lesen und schreiben | Die App kann die Postfacheinstellungen des Benutzers erstellen, lesen, aktualisieren und löschen. Umfasst nicht die Berechtigung zum Senden von E-Mails.|
| _offline_access_ |    Jederzeit auf Daten des Benutzers zugreifen (Vorschau) | Die App kann Benutzerdaten lesen und aktualisieren, auch wenn diese die App derzeit nicht verwenden.|
| _openid_ |    Benutzer anmelden in (Vorschau) | Damit können Benutzer sich mit Ihren Geschäfts- oder Schulkonten bei der App anmelden, und die App kann grundlegende Benutzerprofilinformationen lesen.|
| _User.Read_       |    Anmelden und Benutzerprofil lesen | Damit können Benutzer sich bei der App anmelden, und die App kann das Profil von angemeldeten Benutzern lesen. Das vollständige Profil enthält alle deklarierten Eigenschaften der Benutzer-Entität. Die App kann keine Navigationseigenschaften lesen, z. B. Manager- oder direkte Berichte. Ermöglicht außerdem der App das Lesen der folgenden grundlegenden Firmeninformationen des angemeldeten Benutzers (über das **TenantDetail**-Objekt): Mandanten-ID, Mandantenanzeigename und überprüfte Domänen.|
| _User.ReadWrite_ |    Lese- und Schreibzugriff auf Benutzerprofile | Die App kann Ihr Profil lesen. Darüber hinaus kann die App Ihre Profilinformationen in Ihrem Namen aktualisieren. |
| _User.ReadBasic.All_ |    Lesezugriff auf einfache Profile aller Benutzer | Ermöglicht der App das Lesen der grundlegenden Profile aller Benutzer in der Organisation im Namen des angemeldeten Benutzers. Das grundlegende Profil eines Benutzers umfasst nur die folgenden Eigenschaften: Anzeigename, Vor- und Nachname, Foto und E-Mail-Adresse. Um die Gruppen zu lesen, in denen ein Benutzer Mitglied ist, benötigt die App auch „Group.Read.All“ oder „Group.ReadWrite.All“.| 

###<a name="app-only-permissions-requiring-administrators-consent"></a>Nur-App-Berechtigungen, die die Zustimmung des Administrators erfordern

|   **Bereich**    |  **Berechtigung**   |  **Beschreibung** |
|:---------------|:------------------|:-----------------|
| _Calendars.Read_ |    Lesezugriff auf Kalender in allen Postfächern | Die App kann Ereignisse aller Kalender ohne angemeldeten Benutzer lesen. |
| _Calendars.ReadWrite_ |    Lese- und Schreibzugriff auf Kalender in allen Postfächern | Die App kann Ereignisse aller Kalender ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen.|
| _Contacts.Read_ |    Lesezugriff auf Kontakte in allen Postfächern | Die App kann alle Kontakte in allen Postfächern ohne angemeldeten Benutzer lesen. |
| _Contacts.ReadWrite_ |    Lese- und Schreibzugriff auf Kontakte in allen Postfächern  |Die App kann alle Kontakte in allen Postfächern ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen.|
| _Device.ReadWrite.All_ | Geräteeigenschaften lesen und schreiben | Die App kann alle Geräteeigenschaften ohne angemeldeten Benutzer lesen und schreiben. Ermöglicht nicht das Erstellen oder  Löschen von Geräten oder das Aktualisieren von alternativen Sicherheits-IDs von Geräten. |
| _Directory.Read.All_ | Verzeichnisdaten lesen | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation ohne angemeldeten Benutzer zu lesen, z. B. Benutzer, Gruppen und Apps. |
| _Directory.ReadWrite.All_ | Schreib-/Lesezugriff auf Verzeichnisdaten | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation ohne angemeldeten Benutzer zu lesen und zu schreiben, z. B. Benutzer und Gruppen. Ermöglicht nicht das Löschen eines Benutzers oder einer Gruppe. |
| _Files.Read.All_ | Alle Dateien lesen, auf die der Benutzer zugreifen kann | Die App kann alle Dateien in allen Websitesammlungen ohne angemeldeten Benutzer lesen. |
| _Files.ReadWrite.All_ | Vollzugriff auf alle Dateien, auf die Benutzer zugreifen können | Die App kann alle Dateien in allen Websitesammlungen ohne angemeldeten Benutzer lesen, erstellen, aktualisieren und löschen. |
| _Group.Read.All_ | Lesezugriff auf alle Gruppen | Die App kann Mitgliedschaften für alle Gruppen ohne angemeldeten Benutzer lesen. Beachten Sie, dass nicht alle Gruppen-APIs Zugriff über Nur-App-Berechtigungen unterstützen. Beispiele finden Sie unter [Bekannte Probleme](../overview/release_notes.md#groups). |
| _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen | Die App kann Gruppen erstellen, Gruppenmitgliedschaften lesen und aktualisieren und Gruppen löschen. Alle diese Vorgänge können von der App ohne angemeldeten Benutzer ausgeführt werden. Beachten Sie, dass nicht alle Gruppen-APIs Zugriff über Nur-App-Berechtigungen unterstützen. Beispiele finden Sie unter [Bekannte Probleme](../overview/release_notes.md#groups).|
| _Mail.Read_       |    Lesezugriff auf E-Mails in allen Postfächern | Die App kann E-Mails in allen Postfächern ohne angemeldeten Benutzer lesen.|
| _Mail.ReadWrite_ |    Lese- und Schreibzugriff auf E-Mails in allen Postfächern | Die App kann E-Mails in allen Postfächern ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen. Umfasst nicht über die Berechtigung zum Senden von E-Mails. |
| _Mail.Send_ |    E-Mails als beliebiger Benutzer senden | Die App kann E-Mails als beliebiger Benutzer ohne angemeldeten Benutzer senden. | 
| _MailboxSettings.ReadWrite_ | Alle Benutzerpostfacheinstellungen lesen und schreiben  | Die App kann Benutzerpostfacheinstellungen ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen. Umfasst nicht die Berechtigung zum Senden von E-Mails. |
| _Member.Read.Hidden_ | Alle ausgeblendeten Mitgliedschaften lesen | Die App kann die Mitgliedschaften ausgeblendeter Gruppen und administrativer Einheiten ohne angemeldeten Benutzer lesen. |
| _Reports.Read.All_ | Alle Verwendungsberichte lesen | Die App kann alle Dienstverwendungsberichte ohne angemeldeten Benutzer lesen. Zu Diensten, die Verwendungsberichte bereitstellen, gehören Office 365 und Azure Active Directory. |
| _User.Read.All_ |    Lesezugriff auf vollständige Profile aller Benutzer | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Gruppenmitgliedschaften, Berichte und Vorgesetzte von anderen Benutzern in Ihrer Organisation ohne angemeldeten Benutzers zu lesen.| 
| _User.ReadWrite.All_ |   Lese- und Schreibzugriff auf vollständige Profile aller Benutzer | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Gruppenmitgliedschaften, Berichten und Vorgesetzten von anderen Benutzern in Ihrer Organisation ohne angemeldeten Benutzer zu lesen und zu schreiben.|


##<a name="permission-scopes-in-preview"></a>Berechtigungsbereiche in der Vorschau

###<a name="permissions-requiring-administrators-consent-preview"></a>Berechtigungen, die die Zustimmung des Administrators erfordern (Vorschau)

|   **Bereich**    |  **Berechtigung**   |  **Beschreibung** |
|:---------------|:------------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Informationen zu Identiätsrisikoereignissen lesen (Vorschau) | Ermöglicht der App, Informationen zu Identitätsrisikoereignissen für alle Benutzer in Ihrer Organisation im Namen des angemeldeten Benutzers zu lesen. |
| _DeviceManagementServiceConfiguration.Read.All_ | Microsoft Intune-Konfiguration lesen (Vorschau) | Ermöglicht der App, Microsoft Intune-Diensteigenschaften, einschließlich der Geräteregistrierung und der Drittanbieter-Dienstverbindungskonfiguration, zu lesen. |
| _DeviceManagementServiceConfiguration.ReadWrite.All_ | Microsoft Intune-Konfiguration lesen und schreiben (Vorschau) | Ermöglicht der App, Microsoft Intune-Diensteigenschaften, einschließlich der Geräteregistrierung und der Drittanbieter-Dienstverbindungskonfiguration, zu lesen und zu schreiben. |
| _DeviceManagementConfiguration.Read.All_ | Microsoft Intune-Gerätekonfiguration und -Richtlinien lesen (Vorschau) | Ermöglicht der App, Eigenschaften der von Microsoft Intune verwalteten Gerätekonfiguration und Richtlinien zur Gerätekompatibilität sowie deren Zuweisung zu Gruppen zu lesen. |
| _DeviceManagementConfiguration.ReadWrite.All_ | Microsoft Intune-Gerätekonfiguration und -Richtlinien lesen und schreiben (Vorschau) | Ermöglicht der App, Eigenschaften der von Microsoft Intune verwalteten Gerätekonfiguration und Richtlinien zur Gerätekompatibilität sowie deren Zuweisung zu Gruppen zu lesen und zu schreiben. |
| _DeviceManagementApps.Read.All_ | Microsoft Intune-Apps lesen (Vorschau) | Ermöglicht der App, die Eigenschaften, Gruppenzuweisungen und Status von Apps, App-Konfigurationen sowie von Microsoft Intune verwaltete Richtlinien zum Schutz von Apps zu lesen. |
| _DeviceManagementApps.ReadWrite.All_ | Microsoft Intune-Apps lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften, Gruppenzuweisungen und Status von Apps, App-Konfigurationen sowie von Microsoft Intune verwaltete Richtlinien zum Schutz von Apps zu lesen und zu schreiben. |
| _DeviceManagementRBAC.Read.All_ | Microsoft Intune-RBAC-Einstellungen lesen (Vorschau) | Ermöglicht der App, die Eigenschaften bezüglich der Einstellungen der rollenbasierten Zugriffssteuerung (RBAC) von Microsoft Intune zu lesen. |
| _DeviceManagementRBAC.ReadWrite.All_ | Microsoft Intune-RBAC-Einstellungen lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften bezüglich der Einstellungen der rollenbasierten Zugriffssteuerung (RBAC) von Microsoft Intune zu lesen und zu schreiben. |
| _DeviceManagementManagedDevices.Read.All_ | Microsoft Intune-Geräte lesen (Vorschau) | Ermöglicht der App, die Eigenschaften der von Microsoft Intune verwalteten Geräte zu lesen. |
| _DeviceManagementManagedDevices.ReadWrite.All_ | Microsoft Intune-Geräte lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften der von Microsoft Intune verwalteten Geräte zu lesen und zu schreiben. Ermöglicht keine Operationen mit großen Auswirkungen, z. B. Remotezurücksetzen und Kennwortzurücksetzung am Gerät des Besitzers. |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | Remoteaktionen mit Auswirkungen auf den Benutzer auf Microsoft Intune-Geräten durchführen (Vorschau) | Ermöglicht der App, Remoteaktionen mit großen Auswirkungen durchzuführen, z. B. das Zurücksetzen des Geräts oder der Kennung auf Geräten, die von Microsoft Intune verwaltet werden. |

###<a name="permissions-not-requiring-administrators-consent-preview"></a>Berechtigungen, die keine Zustimmung des Administrators erfordern (Vorschau)

|   **Bereich**    |  **Berechtigung**   |  **Beschreibung** |
|:---------------|:------------------|:-----------------|
| _Notes.Create_ |    Create pages in users' notebooks (Vorschau) | Die App kann die Titel von Notizbüchern und Abschnitten lesen und neue Seiten, Notizbücher und Abschnitte im Namen des angemeldeten Benutzers erstellen.|
| _Notes.Read_ |    Lesezugriff auf Notizbücher von Benutzern (Vorschau) | Die App kann die Titel von OneNote-Notizbüchern und Abschnitten anzeigen und alle Seiten im Namen des angemeldeten Benutzers lesen. Sie kann keine kennwortgeschützten Abschnitte anzeigen. |
| _Notes.Read.All_ |    Lesezugriff auf alle Notizbücher, auf die der Benutzer Zugriff hat (Vorschau) | Die App kann die Inhalte aller Notizbücher und Abschnitte lesen, auf die der Benutzer zugreifen kann.   Sie kann keine kennwortgeschützten Abschnitte lesen. |
| _Notes.ReadWrite_ |    Lese- und Schreibzugriff auf Notizbücher von Benutzern (Vorschau) | Die App kann die Titel von Notizbüchern und Abschnitten lesen, alle Seiten lesen, alle Seiten schreiben und neue Seiten im Namen des angemeldeten Benutzers erstellen.  Sie kann nicht auf kennwortgeschützte Abschnitte zugreifen. |
| _Notes.ReadWrite.All_ |    Lese- und Schreibzugriff auf alle Notizbücher, auf die der Benutzer Zugriff hat (Vorschau) | Die App kann die Inhalte aller Notizbücher und Abschnitte lesen und schreiben, auf die der Benutzer zugreifen kann.  Sie kann nicht auf kennwortgeschützte Abschnitte zugreifen.|
| _Notes.ReadWrite.CreatedByApp_ |    Eingeschränkter Zugriff auf Notizbücher (Vorschau) | Die App kann die Titel von Notizbüchern und Abschnitten lesen und neue Seiten im Namen des angemeldeten Benutzers erstellen. Darüber hinaus kann die App von der App erstellte Seiten lesen und aktualisieren. |
| _People.Read_ |    Lesezugriff auf Listen mit für den Benutzer relevanten Personen (Vorschau) | Die App kann eine bewertete Liste relevanter Personen des angemeldeten Benutzers lesen. Die Liste enthält lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype).|
| _Sites.Read.All_ |    Lesezugriff auf Artikel in allen Websitesammlungen | Die App kann Dokumente lesen und Elemente in allen Websitesammlungen im Namen des angemeldeten Benutzers aufführen. |
| _Sites.ReadWrite.All_ |    Lese-/Schreibzugriff auf Elemente in allen Websitesammlungen | Die App kann Dokumente bearbeiten oder löschen und Elemente in allen Websitesammlungen im Namen des angemeldeten Benutzers aufführen. |
| _Tasks.Read_ | Benutzeraufgaben lesen | Die App kann Benutzeraufgaben lesen. |
| _Tasks.Read.Shared_ | Benutzeraufgaben und freigegebene Aufgaben lesen | Die App kann Aufgaben lesen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Aufgaben des Benutzers und freigegebener Aufgaben. |
| _Tasks.ReadWrite_ |    Benutzeraufgaben und -pläne erstellen, lesen, aktualisieren und löschen (Vorschau) | Die App kann Aufgaben und Pläne (und darin enthaltene Aufgaben), die dem angemeldeten Benutzer zugewiesen oder für diesen freigegeben sind, erstellen, lesen, aktualisieren und löschen.|
| _Tasks.ReadWrite.Shared_ | Benutzeraufgaben und freigegebene Aufgaben lesen und schreiben | Die App kann Aufgaben erstellen, lesen, aktualisieren und löschen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Aufgaben des Benutzers und freigegebener Aufgaben. |



##<a name="permission-scope-scenarios"></a>Szenarien zu Berechtigungsbereichen
Nachfolgend finden Sie einige App-Szenarien unter Verwendung der Ressourcen `User` und `Group` und den entsprechenden erforderlichen Bereichen. Die folgende Tabelle zeigt die für eine App erforderlichen Berechtigungsbereiche, damit eine App bestimmte Vorgänge ausführen kann. Beachten Sie, dass die Möglichkeit des Ausführens einiger Vorgänge für die App davon abhängig ist, ob der Berechtigungsbereich nur für die App gilt oder delegiert wird, und (im Falle delegierter Berechtigungsbereiche) von den Berechtigungen des angemeldeten Benutzers. 

###<a name="access-scenarios-using-the-user-resource-and-the-required-scopes"></a>Zugriffsszenarien unter Verwendung der User-Ressource und der erforderlichen Bereiche

| **App-Aufgaben, die den Benutzer einbeziehen**     |  **Erforderliche Bereiche** | **Berechtigungen** |
|:-------------------------------|:---------------------|:---------------|
| Die App möchte die grundlegenden Informationen von anderen Benutzern lesen (nur Anzeigename und Bild), um diese bei einer Personenauswahl anzuzeigen.     | _User.ReadBasic.All_  |  Lesezugriff auf einfache Profile aller Benutzer |
| Die App möchte das vollständige Benutzerprofil für den angemeldeten Benutzer lesen (direkt unterstellte Personen, Vorgesetzte usw.).     | _User.Read_ | Anmelden und Lesen von Benutzerprofilen zulassen|
| Die App möchte das vollständige Benutzerprofil aller Benutzer lesen.     | _User.Read.All_ |  Lesezugriff auf vollständige Profile aller Benutzer   |
| Die App möchte Dateien, E-Mails und Kalenderinformationen für den angemeldeten Benutzer lesen.     | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | Anmeldung aktivieren und Lesezugriff auf Benutzerprofil, Lesezugriff auf Benutzerdateien, Lesezugriff auf Benutzer-E-Mails, Lesezugriff auf Benutzerkalender |
| Die App möchte die Dateien des angemeldeten Benutzers (eigene) Dateien und Dateien, die andere Benutzer für den angemeldeten Benutzer (mich) freigegeben haben, lesen. | _User.Read_, _Files.Read_, _Sites.Read.All_ | Anmeldung aktivieren und Benutzerprofile lesen, Dateien von Benutzern lesen, Artikel in allen Websitesammlungen lesen |
| Die App möchte das vollständige Benutzerprofil für den angemeldeten Benutzer lesen und schreiben.     | _User.ReadWrite_ | Lese- und Schreibzugriff auf Benutzerprofile |
| Die App möchte das vollständige Benutzerprofil aller Benutzer lesen und schreiben.     | _User.ReadWrite.All_ | Lese- und Schreibzugriff auf vollständige Profile aller Benutzer |
| Die App möchte Dateien, E-Mails und Kalenderinformationen für den angemeldeten Benutzer lesen und schreiben.     | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  Lese- und Schreibzugriff auf Benutzerprofil, Lese- und Schreibzugriff auf Benutzerprofil, Lese- und Schreibzugriff auf Benutzer-E-Mails, Vollzugriff auf Benutzerkalender |
   

###<a name="access-scenarios-using-the-group-resource-and-the-required-scopes"></a>Zugriffsszenarien unter Verwendung der Group-Ressource und der erforderlichen Bereiche
    
| **App-Aufgaben, die die Gruppe einbeziehen**     |  **Erforderliche Bereiche** |  **Berechtigungen** |
|:-------------------------------|:---------------------|:---------------|
| Die App möchte die grundlegenden Gruppeninformationen (nur Anzeigename und Bild) lesen, um diese bei einer Gruppenauswahl anzuzeigen.     | _Group.Read.All_  | Lesezugriff auf alle Gruppen|
| Die App möchte alle Inhalte in allen Office 365-Gruppen lesen, einschließlich Dateien und Unterhaltungen.  Außerdem muss die App Gruppenmitgliedschaften anzeigen und in der Lage sein, Gruppenmitgliedschaften zu aktualisieren (wenn Besitzer).  |  _Group.Read.All_ | Lesezugriff auf Elemente in allen Websitesammlungen, Lesezugriff auf alle Gruppen|
| Die App möchte alle Inhalte in allen Office 365-Gruppen lesen und schreiben, einschließlich Dateien und Unterhaltungen.  Außerdem muss die App Gruppenmitgliedschaften anzeigen und in der Lage sein, Gruppenmitgliedschaften zu aktualisieren (wenn Besitzer).  |     _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  Lese- und Schreibzugriff auf alle Gruppen, Bearbeiten oder Löschen von Artikeln in allen Websitesammlungen |
| Die App möchte eine Office 365-Gruppe ermitteln (suchen). Der Benutzer kann eine bestimmte Gruppe suchen und aus der Aufzählungsliste eine Gruppe auswählen, damit der Benutzer der Gruppe beitreten kann.     | _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen|
| Die App möchte über AAD Graph eine Gruppe erstellen. |     _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen|
 


