# <a name="microsoft-graph-permissions-reference"></a>Microsoft Graph-Berechtigungsreferenz 
Microsoft Graph macht differenzierte Berechtigungen verfügbar, die den Zugriff von Apps auf Ressourcen wie Benutzer, Gruppen und E-Mails steuern. Als Entwickler entscheiden Sie, welche Berechtigungen für Microsoft Graph Ihre App anfordert. Wenn ein Benutzer sich bei Ihrer App anmeldet, erhält er oder in einigen Fällen ein Administrator die Möglichkeit, diesen Berechtigungen zuzustimmen. Falls der Benutzer zustimmt, erhält Ihre App Zugriff auf die angeforderten Ressourcen und APIs. Für Apps, die ohne angemeldeten Benutzer ausgeführt werden, kann den Berechtigungen während der Installation oder Registrierung der App von einem Administrator vorab zugestimmt werden (vorab genehmigte Apps). 

## <a name="delegated-permissions-application-permissions-and-effective-permissions"></a>Delegierte Berechtigungen, Anwendungsberechtigungen und effektive Berechtigungen
Microsoft Graph verfügt über zwei Arten von Berechtigungen: **Delegierte Berechtigungen** und **Anwendungsberechtigungen**. 

- **Delegierte Berechtigungen** werden von Apps verwendet, die mit angemeldetem Benutzer ausgeführt werden. Bei diesen Apps stimmt der Benutzer oder ein Administrator den von der App angeforderten Berechtigungen zu, und an die App wird die Berechtigung delegiert, als angemeldeter Benutzer zu agieren, wenn sie Aufrufe an Microsoft Graph sendet. Einigen delegierten Berechtigungen kann auch von Benutzern zugestimmt werden, die kein Administrator sind, aber einige höhere Rechte erfordern Administratorzustimmung.  

- **Anwendungsberechtigungen** werden von Apps verwendet, die keinen angemeldeten Benutzer erfordern, z. B. Apps, die als Hintergrunddienste oder Daemons ausgeführt werden.  Anwendungsberechtigungen kann nur von einem Administrator zugestimmt werden. 

_Effektive Berechtigungen_ sind die Berechtigungen, über die Ihre App verfügt, wenn sie Aufrufe an Microsoft Graph sendet. Es ist wichtig, den Unterschied zwischen den delegierten und Anwendungsberechtigungen zu verstehen, die Ihren Apps gewährt werden, und ihren effektiven Berechtigungen beim Senden von Aufrufen an Microsoft Graph.

- Bei delegierten Berechtigungen sind die _effektiven Berechtigungen_ der App die Schnittmenge mit den geringsten Rechten aus den delegierten Berechtigungen, die der App (per Zustimmung) gewährt wurden und den Rechten des derzeit angemeldeten Benutzers. Ihre App kann nie mehr Rechte als der angemeldete Benutzer haben. In Organisationen werden die Rechte des angemeldeten Benutzers ggf. durch eine Richtlinie oder die Mitgliedschaft in einer oder mehreren Administratorrollen bestimmt. Weitere Informationen zu Administratorrollen finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles).<br/><br/>Nehmen wir beispielsweise an, Ihrer App wurde die delegierte Berechtigung _User.ReadWrite.All_ gewährt. Diese Berechtigung gewährt Ihrer App nominell die Berechtigung zum Lesen und Aktualisieren des Profils aller Benutzer in einer Organisation. Wenn der angemeldete Benutzer ein globaler Administrator ist, kann Ihre App das Profil aller Benutzer in der Organisation aktualisieren. Wenn der angemeldete Benutzer jedoch kein Mitglied einer Administratorrolle ist, kann Ihre App nur das Profil des angemeldeten Benutzers aktualisieren. Die Profile anderer Benutzer in der Organisation können nicht von der App aktualisiert werden, da der Benutzer, in dessen Namen die App agieren darf, nicht über diese Rechte verfügt.
  
- Bei Anwendungsberechtigungen sind die _effektiven Berechtigungen_ der App sämtliche Rechte, die die Berechtigung impliziert. Eine App mit der Anwendungsberechtigung _User.ReadWrite.All_ kann beispielsweise das Profil aller Benutzer in der Organisation aktualisieren. 

### <a name="microsoft-graph-permission-names"></a>Microsoft Graph-Berechtigungsnamen
Die Namen von Microsoft Graph-Berechtigungen entsprechen einem einfachen Muster: _Ressource.Vorgang.Einschränkung_. Beispielsweise gewährt _User.Read_ die Berechtigung zum Lesen des Profils des angemeldeten Benutzers, _User.ReadWrite_ gewährt die Berechtigung zum Lesen und Ändern des Profils des angemeldeten Benutzers, und _Mail.Send_ gewährt die Berechtigung zum Senden von E-Mails im Namen des angemeldeten Benutzers. 

Das Element _Einschränkung_ des Namens bestimmt das potenzielle Ausmaß von Zugriff, den Ihre App im Verzeichnis hat. Derzeit unterstützt Microsoft Graph die folgenden Einschränkungen: 

* **All** gewährt der App die Berechtigung, die Vorgänge für alle Ressourcen des angegebenen Typs in einem Verzeichnis auszuführen. Beispielsweise gewährt _User.Read.All_ der App potenziell Rechte zum Lesen der Profile aller Benutzer in einem Verzeichnis. 
* **Shared** gewährt der App die Berechtigung, die Vorgänge für Ressourcen auszuführen, die andere Benutzer für den angemeldeten Benutzer freigegeben haben. Diese Einschränkung wird hauptsächlich für Outlook-Ressourcen wie E-Mail, Kalender und Kontakte verwendet. Beispielsweise gewährt _Mail.Read.Shared_ Rechte zum Lesen von E-Mails im Postfach des angemeldeten Benutzers sowie von E-Mails in Postfächern, die andere Benutzer in der Organisation für den angemeldeten Benutzer freigegeben haben.
* **AppFolder** gewährt der App die Berechtigung, Dateien in einem bestimmten Ordner in OneDrive zu lesen und zu schreiben. Diese Einschränkung ist nur für [Dateiberechtigungen](#files-permissions) verfügbar und gilt nur für Microsoft-Konten.
* Wenn **keine Einschränkung** angegeben wird, kann die App die Vorgänge nur für die Ressourcen ausführen, die im Besitz des angemeldeten Benutzers sind. Beispielsweise gewährt _User.Read_ Rechte zum Lesen nur des Profils des angemeldeten Benutzers, und _Mail.Read_ gewährt die Berechtigung zum Lesen nur der E-Mails im Postfach des angemeldeten Benutzers.

> **Hinweis**: In delegierten Szenarios sind die Ihrer App gewährten effektiven Berechtigungen möglicherweise durch die Rechte des angemeldeten Benutzers in der Organisation eingeschränkt.
> 

### <a name="microsoft-accounts-and-work-or-school-accounts"></a>Microsoft-Konten und Geschäfts-, Schul- oder Unikonten

Nicht alle Berechtigungen gelten für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten. In den **Anmerkungen** für die einzelnen Berechtigungsgruppen finden Sie Informationen darüber, ob eine bestimmte Berechtigung für Microsoft-Konten und/oder Geschäfts-, Schul- oder Unikonten gültig ist. 

### <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>Benutzer- und Gruppensucheinschränkungen für Gastbenutzer in Organisationen

Benutzer- und Gruppensuchfunktionen ermöglichen der App, im Verzeichnis einer Organisation nach beliebigen Benutzern oder Gruppen zu suchen, indem der `/users`- oder `/groups`-Ressourcensatz abgefragt wird (z. B. `https://graph.microsoft.com/v1.0/users`). Diese Funktion steht Administratoren und Benutzern zur Verfügung, nicht jedoch Gastbenutzern. Wenn der angemeldete Benutzer ein Gastbenutzer ist, kann er abhängig von den einer App gewährten Berechtigungen das Profil eines bestimmten Benutzers oder einer bestimmten Gruppe lesen (z. B. `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`); er kann jedoch nicht den `/users`- oder `/groups`-Ressourcensatz abfragen, wodurch potenziell mehr als eine einzelne Ressource zurückgegeben wird. Mit den entsprechenden Berechtigungen kann die App die Profile von Benutzern oder Gruppen lesen, die über Links in Navigationseigenschaften abgerufen werden, beispielsweise `/users/{id}/directReports` oder `/groups/{id}/members`.

---

## <a name="calendars-permissions"></a>Kalenderberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    Benutzerkalender lesen  | Ermöglicht der App, Ereignisse in Benutzerkalendern zu lesen.| Nein |
| _Calendars.Read.Shared_ |    Benutzerkalender und freigegebene Kalender lesen | Ermöglicht der App, Ereignisse in allen Kalendern zu lesen, auf die der Benutzer zugreifen kann, einschließlich delegierter und freigegebener Kalender. | Nein |
| _Calendars.ReadWrite_ |    Vollzugriff auf Benutzerkalender  | Ermöglicht der App, Ereignisse in Benutzerkalendern zu erstellen, zu lesen, zu aktualisieren und zu löschen. | Nein |
| _Calendars.ReadWrite.Shared_ |    Benutzerkalender und freigegebene Kalender lesen und schreiben | Die App kann Ereignisse in allen Kalendern, für die der Benutzer über Zugriffsberechtigungen verfügt, erstellen, lesen, aktualisieren und löschen. Dies umfasst delegierte und freigegebene Kalender.| Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    Lesezugriff auf Kalender in allen Postfächern  | Ermöglicht der App, Ereignisse in allen Kalendern ohne einen angemeldeten Benutzer zu lesen.| Ja |
| _Calendars.ReadWrite_ |    Lese- und Schreibzugriff auf Kalender in allen Postfächern | Ermöglicht der App, Ereignisse in allen Kalendern ohne einen angemeldeten Benutzer zu erstellen, zu lesen, zu aktualisieren und zu löschen.| Ja |

### <a name="remarks"></a>Hinweise

_Calendars.Read.Shared_ und _Calendars.ReadWrite.Shared_ gelten nur für Geschäfts-, Schul- oder Unikonten. Alle anderen Berechtigungen gelten für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten.

### <a name="example-usage"></a>Verwendungsbeispiel

#### <a name="delegated"></a>Delegiert

* _Calendars.Read_: Ereignisse im Kalender des Benutzers zwischen dem 23. April 2017 und dem 29. April 2017 abrufen (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`).
* _Calendars.Read.Shared_: Nach Besprechungszeiten suchen, zu denen alle Teilnehmer verfügbar sind (`POST /users/{id|userPrincipalName}/findMeetingTimes`).
* _Calendars.ReadWrite_: Ein Ereignis zum Kalender des Benutzers hinzufügen (`POST /me/events`).

#### <a name="application"></a>Anwendung

* _Calendars.Read_: Ereignisse im Kalender eines Konferenzraums suchen, sortiert nach bob@contoso.com (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`).
* _Calendars.Read_: Alle Ereignisse im Kalender eines Benutzers für den Monat Mai auflisten (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_: Ein Ereignis für einen Zeitpunkt mit genehmigter Abwesenheit zum Kalender eines Benutzers hinzufügen (`POST /users/{id | userPrincipalName}/events`).
* _Calendars.Send_: Eine Nachricht senden (`POST /users/{id | userPrincipalName}/sendCalendars`).


Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="contacts-permissions"></a>Kontaktberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    Benutzerkontakte lesen  | Ermöglicht der App, Benutzerkontakte zu lesen. | Nein |
| _Contacts.Read.Shared_ |    Benutzerkontakte und freigegebene Kontakte lesen | Ermöglicht der App, Kontakte zu lesen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Kontakte des Benutzers und freigegebener Kontakte. | Nein |
| _Contacts.ReadWrite_ |    Vollzugriff auf Benutzerkontakte  | Ermöglicht der App, Benutzerkontakte zu erstellen, zu lesen, zu aktualisieren und zu löschen. | Nein |
| _Contacts.ReadWrite.Shared_ |    Benutzerkontakte und freigegebene Kontakte lesen und schreiben | Ermöglicht der App, Kontakte zu erstellen, zu lesen, zu aktualisieren und zu löschen, für die der Benutzer über Berechtigungen verfügt, einschließlich der eigenen Kontakte des Benutzers und freigegebener Kontakte.| Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    Lesezugriff auf Kontakte in allen Postfächern | Ermöglicht der App, alle Kontakte in allen Postfächern ohne einen angemeldeten Benutzer zu lesen. | Ja |
| _Contacts.ReadWrite_ |    Lese- und Schreibzugriff auf Kontakte in allen Postfächern  |Ermöglicht der App, alle Kontakte in allen Postfächern ohne einen angemeldeten Benutzer zu erstellen, zu lesen, zu aktualisieren und zu löschen.| Ja |

### <a name="remarks"></a>Hinweise
Für Microsoft-Konten sind nur die delegierten Berechtigungen _Contacts.Read_ und _Contacts.ReadWrite_ gültig. 

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Contacts.Read_: Einen Kontakt aus einem der Kontaktordner der obersten Ebene des angemeldeten Benutzers lesen (`GET /me/contactfolders/{Id}/contacts/{id}`).
* _Contacts.ReadWrite_: Das Kontaktfoto eines Kontakts des angemeldeten Benutzers aktualisieren (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`). 
* _Contacts.ReadWrite_: Kontakte zum Stammordner des angemeldeten Benutzers hinzufügen (`POST /me/contacts`).

#### <a name="application"></a>Anwendung

* _Contacts.Read_: Kontakte aus einem der Kontaktordner der obersten Ebene eines beliebigen Benutzers in der Organisation lesen (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`). 
* _Contacts.ReadWrite_: Das Foto eines beliebigen Kontakts eines beliebigen Benutzers in einer Organisation aktualisieren (`PUT /user/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`). 
* _Contacts.ReadWrite_: Kontakte zum Stammordner eines beliebigen Benutzers in der Organisation hinzufügen (`POST /users/{id | userPrincipalName}/contacts`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="device-permissions"></a>Geräteberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.Read_ | Benutzergeräte lesen | Ermöglicht der App, eine Benutzerliste mit Geräten im Auftrag des angemeldeten Benutzers zu lesen. | Nein |
| _Device.Command_ | Kommunikation mit Benutzergeräten | Ermöglicht der App, im Auftrag des angemeldeten Benutzers auf einem Benutzergerät eine andere App zu starten oder mit einer anderen App zu kommunizieren. | Nein |


#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.ReadWrite.All_ | Geräteeigenschaften lesen und schreiben | Die App kann alle Geräteeigenschaften ohne angemeldeten Benutzer lesen und schreiben. Ermöglicht nicht das Erstellen oder  Löschen von Geräten oder das Aktualisieren von alternativen Sicherheits-IDs von Geräten. | Ja |

### <a name="remarks"></a>Hinweise

Die delegierten Berechtigungen _Device.Read_ und _Device.Command_ gelten nur für persönlichen Microsoft-Konten.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="application"></a>Anwendung

* _Device.ReadWrite.All_: Alle registrierten Geräte in der Organisation lesen (`GET /devices`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="microsoft-intune-device-management-permissions"></a>Berechtigungen für Microsoft Intune-Geräteverwaltung

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

Keine.

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _DeviceManagementServiceConfiguration.Read.All_ | Microsoft Intune-Konfiguration lesen (Vorschau) | Ermöglicht der App, Microsoft Intune-Diensteigenschaften zu lesen, einschließlich der Geräteregistrierung und der Drittanbieter-Dienstverbindungskonfiguration. | Ja |
| _DeviceManagementServiceConfiguration.ReadWrite.All_ | Microsoft Intune-Konfiguration lesen und schreiben (Vorschau) | Ermöglicht der App, Microsoft Intune-Diensteigenschaften zu lesen und zu schreiben, einschließlich der Geräteregistrierung und der Drittanbieter-Dienstverbindungskonfiguration. | Ja |
| _DeviceManagementConfiguration.Read.All_ | Microsoft Intune-Gerätekonfiguration und -Richtlinien lesen (Vorschau) | Ermöglicht der App, Eigenschaften der von Microsoft Intune verwalteten Gerätekonfiguration und Richtlinien zur Gerätekompatibilität sowie deren Zuweisung zu Gruppen zu lesen. | Ja |
| _DeviceManagementConfiguration.ReadWrite.All_ | Microsoft Intune-Gerätekonfiguration und -Richtlinien lesen und schreiben (Vorschau) | Ermöglicht der App, Eigenschaften der von Microsoft Intune verwalteten Gerätekonfiguration und Richtlinien zur Gerätekompatibilität sowie deren Zuweisung zu Gruppen zu lesen und zu schreiben. | Ja |
| _DeviceManagementApps.Read.All_ | Microsoft Intune-Apps lesen (Vorschau) | Ermöglicht der App, die Eigenschaften, Gruppenzuweisungen und Status von Apps, App-Konfigurationen sowie von Microsoft Intune verwaltete Richtlinien zum Schutz von Apps zu lesen. | Ja |
| _DeviceManagementApps.ReadWrite.All_ | Microsoft Intune-Apps lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften, Gruppenzuweisungen und Status von Apps, App-Konfigurationen sowie von Microsoft Intune verwaltete Richtlinien zum Schutz von Apps zu lesen und zu schreiben. | Ja |
| _DeviceManagementRBAC.Read.All_ | Microsoft Intune-RBAC-Einstellungen lesen (Vorschau) | Ermöglicht der App, die Eigenschaften bezüglich der Einstellungen der rollenbasierten Zugriffssteuerung (RBAC) von Microsoft Intune zu lesen. | Ja |
| _DeviceManagementRBAC.ReadWrite.All_ | Microsoft Intune-RBAC-Einstellungen lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften bezüglich der Einstellungen der rollenbasierten Zugriffssteuerung (RBAC) von Microsoft Intune zu lesen und zu schreiben. | Ja |
| _DeviceManagementManagedDevices.Read.All_ | Microsoft Intune-Geräte lesen (Vorschau) | Ermöglicht der App, die Eigenschaften der von Microsoft Intune verwalteten Geräte zu lesen. | Ja |
| _DeviceManagementManagedDevices.ReadWrite.All_ | Microsoft Intune-Geräte lesen und schreiben (Vorschau) | Ermöglicht der App, die Eigenschaften der von Microsoft Intune verwalteten Geräte zu lesen und zu schreiben. Ermöglicht keine Operationen mit großen Auswirkungen, z. B. Remotezurücksetzen und Kennwortzurücksetzung am Gerät des Besitzers. | Ja |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | Remoteaktionen mit Auswirkungen auf den Benutzer auf Microsoft Intune-Geräten durchführen (Vorschau) | Ermöglicht der App, Remoteaktionen mit großen Auswirkungen durchzuführen, z. B. das Zurücksetzen des Geräts oder der Kennung auf Geräten, die von Microsoft Intune verwaltet werden. | Ja |

### <a name="remarks"></a>Hinweise
> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Berechtigungen gelten nur für Geschäfts-, Schul- oder Unikonten.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="application"></a>Anwendung

* _DeviceManagementServiceConfiguration.Read.All_: Den aktuellen Status des Intune-Abonnements überprüfen (`GET /deviceManagement/subscriptionState`)
* _DeviceManagementServiceConfiguration.ReadWrite.All_: Neue Geschäftsbedingungen erstellen (`POST /deviceManagement/termsAndConditions`)
* _DeviceManagementConfiguration.Read.All_: Den Status einer Gerätekonfiguration suchen (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)
* _DeviceManagementConfiguration.ReadWrite.All_: Einer Gruppe eine Gerätekompatibilitätsrichtlinie zuweisen (`POST deviceCompliancePolicies/{id}/assign`)
* _DeviceManagementApps.Read.All_: Alle Windows Store-Apps suchen, die in Intune veröffentlicht wurden (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)
* _DeviceManagementApps.ReadWrite.All_: Eine neue Anwendung veröffentlichen (`POST /deviceAppManagement/mobileApps`)
* _DeviceManagementRBAC.Read.All_: Eine Rollenzuweisung anhand des Namens suchen (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)
* _DeviceManagementRBAC.ReadWrite.All_: Eine neue benutzerdefinierte Rolle erstellen (`POST /deviceManagement/roleDefinitions`)
* _DeviceManagementManagedDevices.Read.All_: Ein verwaltetes Gerät anhand des Namens suchen (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)
* _DeviceManagementManagedDevices.ReadWrite.All_: Ein verwaltetes Gerät entfernen (`DELETE /managedDevices/{id}`)
* _DeviceManagementManagedDevices.PrivilegedOperations.All_: Die Kennung auf dem verwalteten Gerät eines Benutzers zurücksetzen (`POST /managedDevices/{id}/resetPasscode`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="directory-permissions"></a>Verzeichnisberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_           |     Verzeichnisdaten lesen                     | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation zu lesen, z. B. Benutzer, Gruppen und Apps. | Ja |
| _Directory.ReadWrite.All_      |     Schreib-/Lesezugriff auf Verzeichnisdaten           | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen und zu schreiben, z. B. Benutzer und Gruppen.  Ermöglicht der App nicht das Löschen von Benutzern oder Gruppen oder das Zurücksetzen von Benutzerkennwörtern. | Ja |
| _Directory.AccessAsUser.All_   |     Als der angemeldete Benutzer auf das Verzeichnis zugreifen  | Ermöglicht der App den gleichen Zugriff auf Informationen im Verzeichnis wie dem angemeldeten Benutzer.| Ja |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | Verzeichnisdaten lesen | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen, z. B. Benutzer, Gruppen und Apps. | Ja |
| _Directory.ReadWrite.All_ | Schreib-/Lesezugriff auf Verzeichnisdaten | Ermöglicht der App, Daten im Verzeichnis Ihrer Organisation ohne angemeldeten Benutzer zu lesen und zu schreiben, z. B. Benutzer und Gruppen. Ermöglicht nicht das Löschen eines Benutzers oder einer Gruppe. | Ja |

### <a name="remarks"></a>Bemerkungen
Verzeichnisberechtigungen werden für Microsoft-Konten nicht unterstützt. 

 Verzeichnisberechtigungen stellen die höchste Stufe von Rechten für den Zugriff auf Verzeichnisressourcen wie [Benutzer](../api-reference/v1.0/resources/user.md), [Gruppen](../api-reference/v1.0/resources/group.md), und [Geräte](../api-reference/v1.0/resources/device.md) in einer Organisation bereit. Sie steuern zudem exklusiv den Zugriff auf andere Verzeichnisressourcen wie [Organisationskontakte](../api-reference/beta/resources/orgcontact.md), [Schemaerweiterungs-APIs](../api-reference/beta/resources/schemaextension.md), [Privileged Identity Management (PIM)-APIs](../api-reference/beta/resources/privilegedidentitymanagement_root.md) sowie viele der Ressourcen und APIs, die unter dem Knoten **Azure Active Directory** in der API-Referenzdokumentation der Versionen 1.0 und Beta aufgeführt sind. Hierzu zählen administrative Einheiten, Verzeichnisrollen, Verzeichniseinstellungen, Richtlinien und viele weitere. 

Die Berechtigung _Directory.ReadWrite.All_ gewährt die folgenden Rechte:

- Alles lesen für alle Verzeichnisressourcen (deklarierte Eigenschaften und Navigationseigenschaften)
- Benutzer erstellen und aktualisieren
- Benutzer deaktivieren und aktivieren (außer Unternehmensadministrator)
- Alternative Sicherheits-ID für Benutzer festlegen (außer Administratoren)
- Gruppen erstellen und aktualisieren
- Gruppenmitgliedschaften verwalten
- Gruppenbesitzer aktualisieren
- Lizenzzuweisungen verwalten
- Schemaerweiterungen für Anwendungen definieren
- **Hinweis**: Keine Rechte zum Zurücksetzen von Benutzerkennwörtern
- **Hinweis**: Keine Rechte zum Löschen von Ressourcen (einschließlich Benutzer oder Gruppen)
- **Hinweis**: Schließt ausdrücklich das Erstellen oder Aktualisieren von Ressourcen aus, die oben nicht aufgeführt sind. Hierzu gehören: application, oAauth2Permissiongrant, appRoleAssignment, device, servicePrincipal, organization, domains usw.
 

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert
* _Directory.Read.All_: Alle administrativen Einheiten in einer Organisation auflisten (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_: Mitglieder zu einer Verzeichnisrolle hinzufügen (`POST /directoryRoles/{id}/members/$ref`)

#### <a name="application"></a>Anwendung
* _Directory.Read.All_: Alle Mitgliedschaften eines Benutzers auflisten, einschließlich Verzeichnisrollen und administrativer Einheiten (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_: Alle Gruppenmitglieder auflisten, einschließlich Dienstprinzipale (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_: Einen Besitzer zu einer Gruppe hinzufügen (`POST /groups/{id}/owners/$ref`)


Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="files-permissions"></a>Dateiberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read_ |    Lesezugriff auf Benutzerdateien | Ermöglicht der App, die Dateien des angemeldeten Benutzers zu lesen.| Nein |
| _Files.Read.All_ | Alle Dateien lesen, auf die der Benutzer zugreifen kann | Ermöglicht der App, alle Dateien zu lesen, auf die der angemeldete Benutzer zugreifen kann. | Nein |
| _Files.ReadWrite_ |   Vollzugriff auf Benutzerdateien | Ermöglicht der App, Dateien des angemeldeten Benutzers zu lesen, zu erstellen, zu aktualisieren und zu löschen. | Nein |
| _Files.ReadWrite.All_ | Vollzugriff auf alle Dateien, auf die Benutzer zugreifen können | Ermöglicht der App, alle Dateien zu lesen, zu erstellen, zu aktualisieren und zu löschen, auf die der angemeldete Benutzer zugreifen kann. | Nein |
| _Files.ReadWrite.AppFolder_ | Vollzugriff auf den Anwendungsordner (Vorschau) | (Vorschau) Ermöglicht der App, Dateien im Anwendungsordner zu lesen, zu erstellen, zu aktualisieren und zu löschen. | Nein |
| _Files.Read.Selected_ |    Dateien lesen, die der Benutzer auswählt (Vorschau) | **Eingeschränkte Unterstützung in Microsoft Graph – siehe Anmerkungen** <br/> (Vorschau) Ermöglicht der App, Dateien zu lesen, die der Benutzer auswählt. Sobald der Benutzer eine Datei auswählt, erhält die App mehrere Stunden Zugriff auf diese Datei. | Nein |
| _Files.ReadWrite.Selected_ |    Dateien lesen und schreiben, die der Benutzer auswählt (Vorschau) | **Eingeschränkte Unterstützung in Microsoft Graph – siehe Anmerkungen** <br/> (Vorschau) Ermöglicht der App, Dateien zu lesen und zu schreiben, die der Benutzer auswählt. Sobald der Benutzer eine Datei auswählt, erhält die App mehrere Stunden Zugriff auf diese Datei. | Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read.All_ | Lesen von Dateien in allen Websitesammlungen (Vorschau) | (Vorschau) Ermöglicht der App, alle Dateien in allen Websitesammlungen ohne einen angemeldeten Benutzer zu lesen. | Ja |
| _Files.ReadWrite.All_ | Lesen und Schreiben von Dateien in allen Websitesammlungen (Vorschau) | **Eingeschränkte Unterstützung in Microsoft Graph** <br/> (Vorschau) Ermöglicht der App, alle Dateien in allen Websitesammlungen ohne einen angemeldeten Benutzer zu lesen, zu erstellen, zu aktualisieren und zu löschen. | Ja |

### <a name="remarks"></a>HinwBemerkungeneise

Die delegierten Berechtigungen „Files.Read“, „Files.ReadWrite“, „Files.Read.All“ und „Files.ReadWrite.All“ sind sowohl für persönliche Microsoft-Konten als auch Geschäfts-, Schul- oder Unikonten gültig. Beachten Sie, dass bei persönlichen Konten „Files.Read“ und „Files.ReadWrite“ auch Zugriff auf Dateien gewähren, die für den angemeldeten Benutzer freigegeben sind. 

Die delegierten Berechtigungen „Files.Read.Selected“ und „Files.ReadWrite.Selected“ sind nur für Geschäfts-, Schul- oder Unikonten gültig und werden nur für Arbeit mit [Office 365-Dateihandlern (v1.0)](https://msdn.microsoft.com/office/office365/howto/using-cross-suite-apps) bereitgestellt. Sie dürfen nicht verwendet werden, um Microsoft Graph-APIs direkt aufzurufen. 

Die delegierte Berechtigung „Files.ReadWrite.AppFolder“ ist nur für persönliche Konten gültig und wird zum Zugreifen auf den [speziellen Anwendungsstammordner](https://dev.onedrive.com/items/special_folders.htm) mit der Microsoft Graph-API [Speziellen Ordner abrufen](../api-reference/v1.0/api/drive_special.md) für OneDrive verwendet.

Die Berechtigung „Files.ReadWrite.All“ unterstützt noch nicht die Microsoft Graph-API [Wiederaufnehmbare Uploadsitzung erstellen](../api-reference/v1.0/api/item_createuploadsession.md) für OneDrive. Vollständige Unterstützung wird in Kürze bereitgestellt. 

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Files.Read_: Dateien lesen, die im OneDrive des angemeldeten Benutzers gespeichert sind (`GET /me/drive/root/children`)
* _Files.Read.All_: Dateien lesen, die für den angemeldeten Benutzer freigegeben sind (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_: Eine Datei im OneDrive des angemeldeten Benutzers schreiben (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_: Eine für den Benutzer freigegebene Datei schreiben (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_: Dateien in den App-Ordner in OneDrive schreiben (`PUT /me/drive/special/approot/children/file.txt/content`)

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="group-permissions"></a>Gruppenberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ |    Lesezugriff auf alle Gruppen | Die App kann Gruppen aufführen und deren Eigenschaften sowie alle Gruppenmitgliedschaften im Namen des angemeldeten Benutzers lesen.  Die App kann außerdem, den Kalender, Unterhaltungen, Dateien und andere Gruppeninhalte für alle Gruppen, auf die der Benutzer zugreifen kann, lesen. | Ja |
| _Group.ReadWrite.All_ |    Schreib-/Lesezugriff auf alle Gruppen| Die App kann Gruppen erstellen und alle Gruppeneigenschaften und -mitgliedschaften im Namen des angemeldeten Benutzers lesen.  Darüber hinaus können Gruppenbesitzer ihre eigenen Gruppen verwalten, und Gruppenmitglieder können Gruppeninhalte aktualisieren. | Ja |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | Lesezugriff auf alle Gruppen | Die App kann Mitgliedschaften für alle Gruppen ohne angemeldeten Benutzer lesen. Beachten Sie, dass nicht alle Gruppen-APIs Zugriff über Nur-App-Berechtigungen unterstützen. Beispiele finden Sie unter [Bekannte Probleme](../concepts/known_issues.md). | Ja |
| _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen | Die App kann Gruppen erstellen, Gruppenmitgliedschaften lesen und aktualisieren und Gruppen löschen. Alle diese Vorgänge können von der App ohne angemeldeten Benutzer ausgeführt werden. Beachten Sie, dass nicht alle Gruppen-APIs Zugriff über Nur-App-Berechtigungen unterstützen. Beispiele finden Sie unter [Bekannte Probleme](../concepts/known_issues.md).| Ja |


### <a name="remarks"></a>Bemerkungen

Gruppenfunktionen werden für Microsoft-Konten nicht unterstützt. 

Für Office 365-Gruppen gewähren Gruppenberechtigungen der App Zugriff auf den Inhalt der Gruppe, z. B. Unterhaltungen, Dateien, Notizen usw. Gruppenberechtigungen werden auch verwendet, um den Zugriff auf [Microsoft Planner](../api-reference/beta/resources/planner_overview.md)-Ressourcen und -APIs zu steuern.

Im Hinblick auf Anwendungsberechtigungen gelten einige Einschränkungen für die unterstützten APIs. Weitere Informationen finden Sie unter [bekannte Probleme](../concepts/known_issues.md).

In einigen Fällen benötigt eine App eventuell [Verzeichnisberechtigungen](#directory-permissions), um einige Gruppeneigenschaften wie `member` und `memberOf` zu lesen. Wenn eine Gruppe z. B. einen oder mehrere [servicePrincipals](../api-reference/beta/resources/serviceprincipal.md) als Mitglieder besitzt, benötigt die App effektive Berechtigungen zum Lesen von Dienstprinzipalen, indem ihr eine der Berechtigungen vom Typ _Directory.\*_ gewährt wird, andernfalls gibt Microsoft Graph einen Fehler zurück. (Im Fall von delegierten Berechtigungen benötigt der angemeldete Benutzer außerdem ausreichende Rechte in der Organisation zum Lesen von Dienstprinzipalen.) Dasselbe gilt für die Eigenschaft `memberOf`, die [administrativeUnits](../api-reference/beta/resources/administrativeunit.md) zurückgeben kann.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Group.Read.All_: Alle Office 365-Gruppen lesen, in denen der angemeldete Benutzer Mitglied ist (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`).
* _Group.Read.All_: Alle Office 365-Gruppeninhalte lesen, wie z. B. Unterhaltungen (`GET /groups/{id}/conversations`).
* _Group.ReadWrite.All_: Gruppeneigenschaften wie Fotos aktualisieren (`PUT /groups/{id}/photo/$value`).
* _Group.ReadWrite.All_: Gruppenmitglieder aktualisieren (`POST /groups/{id}/members/$ref`). HINWEIS: Diese Berechtigung erfordert auch _User.ReadBasic.All_ zum Lesen des Benutzers, der als Mitglied hinzugefügt werden soll.

#### <a name="application"></a>Anwendung

* _Group.Read.All_: Alle Gruppen suchen, deren Name mit „Sales“ beginnt (`GET /groups?$filter=startswith(displayName,'Sales')`).
* _Group.ReadWrite.All_: Daemondienst erstellt neue Ereignisse im Kalender einer Office 365-Gruppe (`POST /groups/{id}/events`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="identity-risk-event-permissions"></a>Berechtigungen für Identitätsrisikoereignisse

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Informationen zu Identitätsrisikoereignissen lesen  | Ermöglicht der App, Informationen zu Identitätsrisikoereignissen für alle Benutzer in Ihrer Organisation im Namen des angemeldeten Benutzers zu lesen. | Ja |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Informationen zu Identitätsrisikoereignissen lesen | Ermöglicht der App, Informationen zu Identitätsrisikoereignissen für alle Benutzer in Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen. | Ja |


### <a name="remarks"></a>HinwBemerkungeneise

_IdentityRiskEvent.Read.All_ gilt nur für Geschäfts-, Schul- oder Unikonten. Damit eine App mit delegierten Berechtigungen Informationen zu Identitätsrisiken lesen kann, muss der angemeldete Benutzer ein Mitglied einer der folgenden Administratorrollen sein: Globaler Administrator, Sicherheitsadministrator oder Benutzer mit Leseberechtigung für Sicherheitsfunktionen Weitere Informationen zu Administratorrollen finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated-and-application"></a>Delegiert und Anwendung
Die folgenden Verwendungen sind für delegierte und Anwendungsberechtigungen gültig:

* Alle Risikoereignisse lesen, die für alle Benutzer im Mandanten generiert werden (`GET /beta/identityRiskEvents`)
* Schadsoftware-Risikoereignisse lesen, die vom Dorknet-Botnet generiert werden (`GET /beta/malwareRiskEvents?$filter=malwareName eq 'Dorkbot'`)
* Die letzten 50 Risikoereignisse lesen (`GET /beta/identityRiskEvents?$orderBy=riskEventDateTime desc&top=50`)
 
Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="mail-permissions"></a>E-Mail-Berechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_ |    Benutzer-E-Mails lesen | Die App kann E-Mails in Benutzerpostfächern lesen. | Nein |
| _Mail.ReadWrite_ |    Schreib-/Lesezugriff auf Benutzer-E-Mails | Die App kann E-Mails in Benutzerpostfächern erstellen, lesen, aktualisieren und löschen. Umfasst nicht über die Berechtigung zum Senden von E-Mails.| Nein |
| _Mail.Read.Shared_ |    Benutzer-E-Mails und freigegebene E-Mails lesen | Die App kann E-Mails lesen, auf die der Benutzer zugreifen kann, einschließlich der eigenen E-Mails des Benutzers und freigegebener E-Mails. | Nein |
| _Mail.ReadWrite.Shared_ |    Benutzer-E-Mails und freigegebene E-Mails lesen und schreiben | Die App kann E-Mails erstellen, lesen, aktualisieren und löschen, für die der Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen E-Mails des Benutzers und freigegebener E-Mails. Umfasst nicht die Berechtigung zum Senden von E-Mails. | Nein |
| _Mail.Send_ |    E-Mails als Benutzer senden | Die App kann E-Mails im Namen der Benutzer in der Organisation zu senden. | Nein |
| _Mail.Send.Shared_ |    Senden von E-Mails im Auftrag von anderen Benutzern | Die App kann E-Mails als angemeldeter Benutzer senden, einschließlich Versand im Namen anderer Benutzer. | Nein |
| _MailboxSettings.Read_ |  Postfacheinstellungen des Benutzers lesen | Die App kann die Postfacheinstellungen des Benutzers lesen. Umfasst nicht die Berechtigung zum Senden von E-Mails. | Nein |
| _MailboxSettings.ReadWrite_ |  Benutzerpostfacheinstellungen lesen und schreiben | Die App kann die Postfacheinstellungen des Benutzers erstellen, lesen, aktualisieren und löschen. Umfasst nicht die Berechtigung zum Senden von E-Mails. | Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_       |    Lesezugriff auf E-Mails in allen Postfächern | Die App kann E-Mails in allen Postfächern ohne einen angemeldeten Benutzer lesen.| Ja |
| _Mail.ReadWrite_ |    Lese- und Schreibzugriff auf E-Mails in allen Postfächern | Die App kann E-Mails in allen Postfächern ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen. Umfasst nicht über die Berechtigung zum Senden von E-Mails. | Ja |
| _Mail.Send_ |    E-Mails als beliebiger Benutzer senden | Die App kann E-Mails im Namen eines beliebigen Benutzers ohne einen angemeldeten Benutzer senden. | Ja | 
| _MailboxSettings.Read_ |  Alle Benutzerpostfacheinstellungen lesen | Die App kann Benutzerpostfacheinstellungen ohne einen angemeldeten Benutzer lesen. Umfasst nicht die Berechtigung zum Senden von E-Mails. | Nein |
| _MailboxSettings.ReadWrite_ | Alle Benutzerpostfacheinstellungen lesen und schreiben  | Die App kann Benutzerpostfacheinstellungen ohne angemeldeten Benutzer erstellen, lesen, aktualisieren und löschen. Umfasst nicht die Berechtigung zum Senden von E-Mails. | Ja |

### <a name="remarks"></a>Hinweise

_Mail.Read.Shared_, _Mail.ReadWrite.Shared_ und _Mail.Send.Shared_ gelten nur für Geschäfts-, Schul- oder Unikonten. Alle anderen Berechtigungen gelten für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten.

Mit der Berechtigung _Mail.Send_ oder _Mail.Send.Shared_ kann eine App E-Mails senden und eine Kopie im Ordner „Gesendete Elemente“ des Benutzers speichern, selbst wenn die App keine entsprechende _Mail.ReadWrite_- oder _Mail.ReadWrite.Shared_-Berechtigung verwendet.

### <a name="example-usage"></a>Verwendungsbeispiel

#### <a name="delegated"></a>Delegiert

* _Mail.Read_: Nachrichten im Posteingang des Benutzers sortiert nach `receivedDateTime` auflisten (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`).
* _Mail.Read.Shared_: Aller Nachrichten mit Anlagen im Posteingang eines Benutzers suchen, der seinen Posteingang für den angemeldeten Benutzer freigegeben hat (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`).
* _Mail.ReadWrite_: Eine Nachricht als gelesen markieren (`PATCH /me/messages/{id}`).
* _Mail.Send_: Eine Nachricht senden (`POST /me/sendmail`).
* _MailboxSettings.ReadWrite_: Die automatische Antwort des Benutzers aktualisieren (`PATCH /me/mailboxSettings`).

#### <a name="application"></a>Anwendung

* _Mail.Read_: Nachrichten von bob@contoso.com suchen (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`).
* _Mail.ReadWrite_: Einen neuen Ordner mit dem Namen `Expense Reports` im Posteingang erstellen (`POST /users/{id | userPrincipalName}/mailfolders`).
* _Mail.Send_: Eine Nachricht senden (`POST /users/{id | userPrincipalName}/sendmail`).
* _MailboxSettings.Read_: Die Standardzeitzone für das Postfach des Benutzers abrufen (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="member-permissions"></a>Mitgliedsberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

Keine.

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Member.Read.Hidden_ | Alle ausgeblendeten Mitgliedschaften lesen | Ermöglicht der App, die Mitgliedschaften ausgeblendeter Gruppen und administrativer Einheiten ohne einen angemeldeten Benutzer zu lesen. | Ja |

### <a name="remarks"></a>Hinweise
Die Mitgliedschaft in einigen Office 365-Gruppen kann ausgeblendet werden. Dies bedeutet, dass nur die Mitglieder der Gruppe deren Mitglieder anzeigen können. Dieses Feature ist hilfreich zur Einhaltung von Vorschriften, die erfordern, dass eine Organisation Gruppenmitgliedschaften für Außenstehende ausblendet (z. B. eine Office 365-Gruppe, zu der in einem Kurs angemeldete Teilnehmer gehören).

### <a name="example-usage"></a>Verwendungsbeispiel

#### <a name="application"></a>Anwendung

* _Member.Read.Hidden_: Die Mitglieder einer administrativen Einheit mit ausgeblendeter Mitgliedschaft lesen (`GET /administrativeUnits/{id}/members`).
* _Member.Read.Hidden_: Die Mitglieder einer Gruppe mit ausgeblendeter Mitgliedschaft lesen (`GET /groups/{id}/members`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="notes-permissions"></a>Notizberechtigungen
#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read_ |    OneNote-Benutzernotizbücher lesen | Ermöglicht der App, die Titel von OneNote-Notizbüchern und -Abschnitten zu lesen sowie neue Seiten, Notizbücher und Abschnitte im Namen des angemeldeten Benutzers zu erstellen. | Nein |
| _Notes.Create_ |    OneNote-Benutzernotizbücher erstellen | Ermöglicht der App, die Titel von OneNote-Notizbüchern und -Abschnitten zu lesen sowie neue Seiten, Notizbücher und Abschnitte im Namen des angemeldeten Benutzers zu erstellen.| Nein |
| _Notes.ReadWrite_ |    OneNote-Benutzernotizbücher lesen und schreiben | Ermöglicht der App, OneNote-Notizbücher im Namen des angemeldeten Benutzers zu lesen, freizugeben und zu ändern. | Nein |
| _Notes.Read.All_ |    Alle OneNote-Notizbücher lesen, auf die der Benutzer zugreifen kann | Ermöglicht der App, OneNote-Notizbücher zu lesen, auf die der angemeldete Benutzer in der Organisation Zugriff hat. | Nein |
| _Notes.ReadWrite.All_ |    Alle OneNote-Notizbücher lesen und schreiben, auf die der Benutzer zugreifen kann | Ermöglicht der App, OneNote-Notizbücher zu lesen, freizugeben und zu ändern, auf die der angemeldete Benutzer in der Organisation Zugriff hat.| Nein |
| _Notes.ReadWrite.CreatedByApp_ |    Eingeschränkter Zugriff auf Notizbücher (veraltet) | **Veraltet** <br/>Nicht verwenden. Durch diese Berechtigung werden keine Rechte gewährt. | Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read.All_ |    Alle OneNote-Benutzernotizbücher lesen | Ermöglicht der App, alle OneNote-Notizbücher in Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen. | Ja |
| _Notes.ReadWrite.All_ |    Alle OneNote-Benutzernotizbücher lesen und schreiben | Ermöglicht der App, alle OneNote-Notizbücher in Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen, freizugeben und zu ändern.| Ja |


### <a name="remarks"></a>HinwBemerkungeneise
_Notes.Read.All_ und _Notes.ReadWrite.All_ gelten nur für Geschäfts-, Schul- oder Unikonten. Alle anderen Berechtigungen gelten für Microsoft-Konten und Geschäfts-, Schul- oder Unikonten.

Mit der Berechtigung _Notes.Create_ kann eine App die OneNote-Notizbuchhierarchie des angemeldeten Benutzers anzeigen und OneNote-Inhalte (Notizbücher, Abschnittsgruppen, Abschnitte, Seiten usw.) erstellen.

_Notes.ReadWrite_ und _Notes.ReadWrite.All_ ermöglichen der App außerdem, die Berechtigungen für den OneNote-Inhalt zu ändern, auf den vom angemeldeten Benutzer zugegriffen werden kann. 

Für Geschäfts-, Schul- oder Unikonten ermöglichen _Notes.Read.All_ und _Notes.ReadWrite.All_ der App, auf OneNote-Inhalte anderer Benutzer zuzugreifen, für die der angemeldete Benutzer innerhalb der Organisation über Berechtigungen verfügt.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Notes.Create_: Ein neues Notizbuch für den angemeldeten Benutzer erstellen (`POST /me/onenote/notebooks`).
* _Notes.Read_: Die Notizbücher des angemeldeten Benutzers lesen (`GET /me/onenote/notebooks`).
* _Notes.Read.All_: Alle Notizbücher abrufen, auf die der angemeldete Benutzer innerhalb der Organisation Zugriff hat (`GET /me/onenote/notebooks?includesharednotebooks=true`).
* _Notes.ReadWrite_: Die Seite des angemeldeten Benutzers aktualisieren (`PATCH /me/onenote/pages/{id}/$value`).
* _Notes.ReadWrite.All_: Eine Seite im Notizbuch eines anderen Benutzers erstellen, auf das der angemeldete Benutzer innerhalb der Organisation Zugriff hat (`POST /users/{id}/onenote/pages`).

#### <a name="application"></a>Anwendung

* _Notes.Read.All_: Alle Benutzernotizbücher in einer Gruppe lesen (`GET /groups/{id}/onenote/notebooks`).
* _Notes.ReadWrite.All_: Die Seite in einem Notizbuch für einen beliebigen Benutzer in der Organisation aktualisieren (`PATCH /users/{id}/onenote/pages/{id}/$value`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="openid-permissions"></a>OpenID-Berechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _email_ |    E-Mail-Adresse von Benutzern anzeigen | Ermöglicht der App, die primäre E-Mail-Adresse Ihrer Benutzer zu lesen. | Nein |
| _offline_access_ |    Jederzeit auf Daten des Benutzers zugreifen | Ermöglicht der App, Benutzerdaten zu lesen und zu aktualisieren, auch wenn diese die App derzeit nicht verwenden.| Nein |
| _openid_ |    Benutzer anmelden | Damit können Benutzer sich mit Ihren Geschäfts- oder Schulkonten bei der App anmelden, und die App kann grundlegende Benutzerprofilinformationen lesen.| Nein |
| _profile_ |    Grundlegendes Profil von Benutzern anzeigen | Ermöglicht der App, das grundlegende Profil Ihrer Benutzer (Name, Bild, Benutzername) anzuzeigen.| Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

Keine.

### <a name="remarks"></a>HinwBemerkungeneise
Sie können diese Berechtigungen verwenden, um Artefakte anzugeben, die in Azure AD-Autorisierungs- und Tokenanforderungen zurückgegeben werden sollen. Sie werden von den Azure AD v1.0- und v2.0-Endpunkten unterschiedlich unterstützt.

Beim Azure AD (v1.0)-Endpunkt wird nur die Berechtigung _openid_ verwendet. Sie wird im *scope*-Parameter in einer Autorisierungsanforderung angegeben, um ein ID-Token zurückzugeben, wenn Sie das OpenID Connect-Protokoll zum Anmelden eines Benutzers bei Ihrer App verwenden. Weitere Informationen finden Sie unter [Autorisieren des Zugriffs auf Webanwendungen mithilfe von Open ID Connect und Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-protocols-openid-connect-code). Damit ein ID-Token erfolgreich zurückgegeben wird, müssen Sie auch sicherstellen, dass die Berechtigung _User.Read_ konfiguriert wird, wenn Sie Ihre App registrieren. 

Beim Azure AD v2.0-Endpunkt geben Sie die Berechtigung _offline\_access_ im _scope_-Parameter an, um explizit ein Aktualisierungstoken anzufordern, wenn Sie das OAuth 2.0- oder OpenID-Protokoll verwenden. Bei OpenID Connect geben Sie die Berechtigung _openid_ zum Anfordern eines ID-Tokens an. Sie können auch die Berechtigung _email_, die Berechtigung _profile_ oder beide angeben, um zusätzliche Ansprüche im ID-Token zurückzugeben. Sie müssen nicht _User.Read_ angeben, um ein ID-Token mit dem v2.0-Endpunkt zurückzugeben. Weitere Informationen finden Sie unter [OpenID Connect -Bereiche](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes).

> **Wichtig** In der MSAL (Microsoft Authentication Library) werden derzeit standardmäßig _offline\_access_, _openid_, _profile_, und _email_  in Autorisierungs- und Tokenanforderungen angegeben. Wenn Sie diese Berechtigungen explizit angeben, bedeutet dies im Standardfall, dass Azure AD möglicherweise einen Fehler zurückgibt.
>  

---

## <a name="people-permissions"></a>Personenberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read_ |    Lesezugriff auf Listen mit für den Benutzer relevanten Personen (Vorschau) | Die App kann eine bewertete Liste relevanter Personen des angemeldeten Benutzers lesen. Die Liste enthält lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype).| Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

Keine.

### <a name="remarks"></a>Bemerkungen


### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert


Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="reports-permissions"></a>Berichtsberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

Keine.

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Reports.Read.All_ | Alle Verwendungsberichte lesen | Die App kann alle Dienstverwendungsberichte ohne angemeldeten Benutzer lesen. Zu Diensten, die Verwendungsberichte bereitstellen, gehören Office 365 und Azure Active Directory. | Ja |

### <a name="remarks"></a>Bemerkungen
Berichtsberechtigungen gelten nur für Geschäfts-, Schul- oder Unikonten. 

### <a name="example-usage"></a>Verwendungsbeispiel

#### <a name="application"></a>Anwendung

* _Reports.Read.All_: Verwendungsdetailbericht von E-Mail-Apps für einen Zeitraum von 7 Tagen lesen (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`)
* _Reports.Read.All_: Aktivitätsdetailbericht von E-Mails mit dem Datum „2017-01-01“ lesen (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`)
* _Reports.Read.All_: Office 365-Aktivierungsdetailbericht lesen (`GET /reports/Office365Activations(view='Detail')/content`)

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="sites-permissions"></a>Websiteberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Sites.Read.All_ |    Elemente in allen Websitesammlungen lesen | Ermöglicht der App, Dokumente und Listenelemente in allen Websitesammlungen im Namen des angemeldeten Benutzers zu lesen. | Nein |
| _Sites.ReadWrite.All_ |    Lese-/Schreibzugriff auf Elemente in allen Websitesammlungen | Ermöglicht der App, Dokumente und Listenelemente in allen Websitesammlungen im Namen des angemeldeten Benutzers zu bearbeiten oder zu löschen. | Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

Keine.

### <a name="remarks"></a>Bemerkungen
Websiteberechtigungen gelten nur für Geschäfts-, Schul- oder Unikonten.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Sites.Read.All_: Die Listen auf der SharePoint-Stammwebsite lesen (`GET /beta/sharePoint/site/lists`)
* _Sites.ReadWrite.All_: Neue Listenelemente in einer SharePoint-Liste erstellen (`POST /beta/sharePoint/site/lists/123/items`)


Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="tasks-permissions"></a>Aufgabenberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Tasks.Read_ | Benutzeraufgaben lesen | Ermöglicht der App, Benutzeraufgaben zu lesen. | Nein |
| _Tasks.Read.Shared_ | Benutzeraufgaben und freigegebene Aufgaben lesen | Ermöglicht der App, Aufgaben zu lesen, für die ein Benutzer über Zugriffsberechtigungen verfügt, einschließlich der eigenen Aufgaben des Benutzers und freigegebener Aufgaben. | Nein |
| _Tasks.ReadWrite_ |    Benutzeraufgaben und -container erstellen, lesen, aktualisieren und löschen | Ermöglicht der App, Aufgaben und Container (und darin enthaltene Aufgaben), die dem angemeldeten Benutzer zugewiesen oder für diesen freigegeben sind, zu erstellen, zu lesen, zu aktualisieren und zu löschen.| Nein |
| _Tasks.ReadWrite.Shared_ | Benutzeraufgaben und freigegebene Aufgaben lesen und schreiben | Ermöglicht der App, Aufgaben zu erstellen, zu lesen, zu aktualisieren und zu löschen, für die ein Benutzer über Berechtigungen verfügt, einschließlich der eigenen Aufgaben des Benutzers und freigegebener Aufgaben. | Nein |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

Keine.

### <a name="remarks"></a>HinwBemerkungeneise
_Aufgaben_berechtigungen werden zum Steuern des Zugriffs für Outlook-Aufgaben verwendet. Der Zugriff auf Microsoft Planner-Aufgaben wird von [ _Gruppen_berechtigungen](#group-permissions) gesteuert.

_Freigegebene_ Berechtigungen werden derzeit nur für Geschäfts-, Schul- oder Unikonten unterstützt. Selbst mit _freigegebenen_ Berechtigungen können Fehler bei Lese- oder Schreibvorgängen auftreten, wenn der Benutzer, dem der freigegebene Inhalt gehört, dem zugreifenden Benutzer keine Berechtigungen zum Ändern von Inhalten im Ordner gewährt hat.

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _Tasks.Read_: Alle Aufgaben im Postfach eines Benutzers abrufen (`GET /me/outlook/tasks`).
* _Tasks.Read.Shared_: Auf Aufgaben in einem Ordner zugreifen, der von einem anderen Benutzer in Ihrer Organisation für Sie freigegeben wurde (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`).
* _Tasks.ReadWrite_: Ein Ereignis zum Standardaufgabenordner des Benutzers hinzufügen (`POST /me/outook/tasks`).
* _Tasks.Read_: Alle unerledigten Aufgaben im Postfach eines Benutzers abrufen (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`).
* _Tasks.ReadWrite_: Eine Aufgabe im Postfach eines Benutzers aktualisieren (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`).
* _Tasks.ReadWrite.Shared_: Eine Aufgabe im Namen eines anderen Benutzers ausführen (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="user-permissions"></a>Benutzerberechtigungen

#### <a name="delegated-permissions"></a>Delegierte Berechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read_       |    Anmelden und Benutzerprofil lesen | Damit können Benutzer sich bei der App anmelden, und die App kann das Profil von angemeldeten Benutzern lesen. Die App kann auch grundlegende Unternehmensinformationen von angemeldeten Benutzern lesen.| Nein |
| _User.ReadWrite_ |    Lese- und Schreibzugriff auf Benutzerprofile | Die App kann Ihr Profil lesen. Darüber hinaus kann die App Ihre Profilinformationen in Ihrem Namen aktualisieren. | Nein |
| _User.ReadBasic.All_ |    Grundlegende Profile aller Benutzer lesen | Ermöglicht der App, einen grundlegenden Satz von Profileigenschaften anderer Benutzer in Ihrer Organisation im Namen des angemeldeten Benutzers zu lesen. Dazu gehören der Anzeigename, der Vor-und Nachname, die E-Mail-Adresse und das Foto. | Nein |
| _User.Read.All_  |     Vollständige Profile aller Benutzer lesen           | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Berichten und Vorgesetzten von anderen Benutzern in Ihrer Organisation im Namen des angemeldeten Benutzers zu lesen. | Ja |
| _User.ReadWrite.All_ |     Lese- und Schreibzugriff auf vollständige Profile aller Benutzer | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Berichten und Vorgesetzten von anderen Benutzern in Ihrer Organisation im Namen des angemeldeten Benutzers zu lesen und zu schreiben. Ermöglicht der App außerdem, im Namen des angemeldeten Benutzers Benutzer zu erstellen und zu löschen sowie Benutzerkennwörter zurückzusetzen. | Ja |
| _User.Invite.All_  |     Gastbenutzer zur Organisation einladen | Ermöglicht der App, Gastbenutzer im Namen des angemeldeten Benutzers zu Ihrer Organisation einzuladen. | Ja |

#### <a name="application-permissions"></a>Anwendungsberechtigungen

|   Berechtigung    |  Anzeigezeichenfolge   |  Beschreibung | Administratorzustimmung erforderlich |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read.All_ |    Lesezugriff auf vollständige Profile aller Benutzer | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Gruppenmitgliedschaften, Berichte und Vorgesetzte von anderen Benutzern in Ihrer Organisation ohne angemeldeten Benutzers zu lesen.| Ja |
| _User.ReadWrite.All_ |   Lese- und Schreibzugriff auf vollständige Profile aller Benutzer | Ermöglicht der App, den vollständigen Satz von Profileigenschaften, Gruppenmitgliedschaften, Berichten und Vorgesetzten von anderen Benutzern in Ihrer Organisation ohne einen angemeldeten Benutzer zu lesen und zu schreiben.  Ermöglicht der App außerdem, Benutzer zu erstellen, die kein Administrator sind. Ermöglicht nicht das Zurücksetzen von Benutzerkennwörtern. | Ja |
| _User.Invite.All_  |     Gastbenutzer zur Organisation einladen | Ermöglicht der App, Gastbenutzer ohne einen angemeldeten Benutzer zu Ihrer Organisation einzuladen. | Ja |

### <a name="remarks"></a>HinwBemerkungeneise

Für Microsoft-Konten sind lediglich die Berechtigungen _User.Read_ und _User.ReadWrite_ gültig. Für Geschäfts-, Schul- oder Unikonten sind alle Berechtigungen gültig.

Mit der Berechtigung _User.Read_ kann eine App auch die grundlegenden Unternehmensinformationen des angemeldeten Benutzers für ein Geschäfts-, Schul- oder Unikonto über die [organization](../api-reference/v1.0/resources/organization.md)-Ressource lesen. Die folgenden Eigenschaften sind verfügbar: id, displayName und verifiedDomains.

Für Geschäfts-, Schul- oder Unikonten enthält das vollständige Profil alle deklarierten Eigenschaften der [User](../api-reference/v1.0/resources/user.md)-Ressource. Bei Lesevorgängen wird standardmäßig nur eine begrenzte Anzahl von Eigenschaften zurückgegeben. Um Eigenschaften zu lesen, die nicht im Standardsatz enthalten sind, verwenden Sie `$select`. Die Standardeigenschaften sind folgende:

- displayName
- givenName
- jobTitle
- mail
- mobilePhone
- officeLocation
- preferredLanguage
- surname
- userPrincipalName

 Die delegierten Berechtigungen _User.ReadWrite_ und _User.Readwrite.All_ ermöglichen der App, die folgenden Profileigenschaften für Geschäfts-, Schul- oder Unikonten zu aktualisieren:

- aboutMe
- birthday
- hireDate
- interests
- mobilePhone
- mySite
- pastProjects
- photo
- preferredName
- responsibilities
- schools
- skills

Mit der Anwendungsberechtigung _User.ReadWrite.All_ kann die App alle deklarierten Eigenschaften von Geschäfts-, Schul- oder Unikonten mit Ausnahme des Kennworts aktualisieren.

Zum Lesen oder Schreiben von direkten Mitarbeitern (`directReports`) oder des Vorgesetzten (`manager`) eines Geschäfts-, Schul- oder Unikontos benötigt die App entweder die Berechtigung _User.Read.All_ (schreibgeschützt) oder _User.ReadWrite.All_.

Die Berechtigung _User.ReadBasic.All_ schränkt den App-Zugriff auf einen begrenzten Satz von Eigenschaften ein, der als grundlegendes Profil bezeichnet wird. Grund hierfür ist, dass das vollständige Profil möglicherweise vertrauliche Verzeichnisinformationen enthält. Das grundlegende Profil umfasst lediglich die folgenden Eigenschaften: 

- displayName
- givenName
- mail
- photo
- surname
- userPrincipalName

Zum Lesen der Gruppenmitgliedschaften eines Benutzers (`memberOf`) benötigt die App entweder die Berechtigung [ _Group.Read.All_ ](#group-permissions) oder [ _Group.ReadWrite.All_](#group-permissions). Wenn der Benutzer jedoch auch Mitglied in einer [directoryRole](../api-reference/v1.0/resources/directoryrole.md) oder [administrativeUnit](../api-reference/beta/resources/administrativeunit.md) ist, benötigt die App außerdem effektive Berechtigungen zum Lesen dieser Ressourcen; andernfalls gibt Microsoft Graph einen Fehler zurück. Dies bedeutet, dass die App auch [Verzeichnisberechtigungen](#directory-permissions) benötigt; für delegierte Berechtigungen benötigt der angemeldete Benutzer außerdem ausreichende Rechte in der Organisation, um auf Verzeichnisrollen und administrative Einheiten zuzugreifen. 

### <a name="example-usage"></a>Verwendungsbeispiel
#### <a name="delegated"></a>Delegiert

* _User.Read_: Das vollständige Profil des angemeldeten Benutzers lesen (`GET /me`).
* _User.ReadWrite_: Das Foto des angemeldeten Benutzers aktualisieren (`PUT /me/photo/$value`).
* _User.ReadBasic.All_: Alle Benutzer suchen, deren Name mit „David“ beginnt (`GET /users?$filter=startswith(displayName,'David')`).
* _User.Read.All_: Den Vorgesetzten eines Benutzers lesen (`GET /user/{id | userPrincipalName}/manager`).


#### <a name="application"></a>Anwendung

* _User.Read.All_: Alle Benutzer und Beziehungen über eine Delta-Abfrage lesen (`GET /beta/users/delta?$select=displayName,givenName,surname`).
* _User.ReadWrite.All_: Das Foto eines beliebigen Benutzers in der Organisation aktualisieren (`PUT /user/{id | userPrincipalName}/photo/$value`).

Komplexere Szenarios, die mehrere Berechtigungen erfordern, finden Sie unter [Berechtigungsszenarios](#permission-scenarios).

---

## <a name="permission-scenarios"></a>Berechtigungsszenarios

In diesem Abschnitt werden einige gängige Szenarios für [user](../api-reference/v1.0/resources/user.md) und [group](../api-reference/v1.0/resources/group.md)-Ressourcen in einer Organisation erläutert. In den Tabellen sind die Berechtigungen aufgeführt, die eine App benötigt, um bestimmte Vorgänge auszuführen, die das Szenario erfordert. Beachten Sie, dass in einigen Fällen die Möglichkeit der App zur Ausführung bestimmter Vorgänge davon abhängig ist, ob eine Berechtigung eine Anwendungs- oder eine delegierte Berechtigung ist. Im Falle von delegierten Berechtigungen hängen die effektiven Berechtigungen der App auch von den Berechtigungen des angemeldeten Benutzers innerhalb der Organisation ab. Weitere Informationen finden Sie unter [Delegierte Berechtigungen, Anwendungsberechtigungen und effektive Berechtigungen](#delegated-permissions-application-permissions-and-effective-permissions).

### <a name="access-scenarios-on-the-user-resource"></a>Zugriffsszenarios für die User-Ressource

| **App-Aufgaben, die den Benutzer betreffen**   |  **Erforderliche Berechtigungen** | **Berechtigungszeichenfolgen** |
|:-------------------------------|:---------------------|:---------------|
| Die App möchte die grundlegenden Informationen von anderen Benutzern lesen (nur Anzeigename und Bild), beispielsweise um diese in einer Personenauswahl anzuzeigen.   | _User.ReadBasic.All_  |  Grundlegende Profile aller Benutzer lesen |
| Die App möchte das vollständige Benutzerprofil des angemeldeten Benutzers lesen (direkte Mitarbeiter, Vorgesetzte usw.).     | _User.Read_ | Anmelden und Lesen von Benutzerprofilen zulassen|
| Die App möchte das vollständige Benutzerprofil aller Benutzer lesen.  | _User.Read.All_ |  Lesezugriff auf vollständige Profile aller Benutzer   |
| Die App möchte Dateien, E-Mails und Kalenderinformationen für den angemeldeten Benutzer lesen.  | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | Anmeldung aktivieren und Lesezugriff auf Benutzerprofil, Lesezugriff auf Benutzerdateien, Lesezugriff auf Benutzer-E-Mails, Lesezugriff auf Benutzerkalender |
| Die App möchte die Dateien des angemeldeten Benutzers (eigene) Dateien und Dateien, die andere Benutzer für den angemeldeten Benutzer (mich) freigegeben haben, lesen. | _User.Read_, _Files.Read_, _Sites.Read.All_ | Anmeldung aktivieren und Benutzerprofile lesen, Dateien von Benutzern lesen, Artikel in allen Websitesammlungen lesen |
| Die App möchte das vollständige Benutzerprofil für den angemeldeten Benutzer lesen und schreiben.   | _User.ReadWrite_ | Lese- und Schreibzugriff auf Benutzerprofile |
| Die App möchte das vollständige Benutzerprofil aller Benutzer lesen und schreiben.    | _User.ReadWrite.All_ | Lese- und Schreibzugriff auf vollständige Profile aller Benutzer |
| Die App möchte Dateien, E-Mails und Kalenderinformationen für den angemeldeten Benutzer lesen und schreiben.    | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  Lese- und Schreibzugriff auf Benutzerprofil, Lese- und Schreibzugriff auf Benutzerprofil, Lese- und Schreibzugriff auf Benutzer-E-Mails, Vollzugriff auf Benutzerkalender |
   

### <a name="access-scenarios-on-the-group-resource"></a>Zugriffsszenarios für die Group-Ressource
    
| **App-Aufgaben, die die Gruppe betreffen**  |  **Erforderliche Berechtigungen** |  **Berechtigungszeichenfolgen** |
|:-------------------------------|:---------------------|:---------------|
| Die App möchte die grundlegenden Gruppeninformationen (nur Anzeigename und Bild) lesen, beispielsweise um diese in einer Gruppenauswahl anzuzeigen.  | _Group.Read.All_  | Lesezugriff auf alle Gruppen|
| Die App möchte alle Inhalte in allen Office 365-Gruppen lesen, einschließlich Dateien und Unterhaltungen.  Außerdem muss die App Gruppenmitgliedschaften anzeigen und in der Lage sein, Gruppenmitgliedschaften zu aktualisieren (wenn Besitzer).  |  _Group.Read.All_ | Lesezugriff auf Elemente in allen Websitesammlungen, Lesezugriff auf alle Gruppen|
| Die App möchte alle Inhalte in allen Office 365-Gruppen lesen und schreiben, einschließlich Dateien und Unterhaltungen.  Außerdem muss die App Gruppenmitgliedschaften anzeigen und in der Lage sein, Gruppenmitgliedschaften zu aktualisieren (wenn Besitzer).  |   _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  Lese- und Schreibzugriff auf alle Gruppen, Bearbeiten oder Löschen von Artikeln in allen Websitesammlungen |
| Die App möchte eine Office 365-Gruppe ermitteln (suchen). Der Benutzer kann eine bestimmte Gruppe suchen und aus der Aufzählungsliste eine Gruppe auswählen, damit der Benutzer der Gruppe beitreten kann.     | _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen|
| Die App möchte über AAD Graph eine Gruppe erstellen. |   _Group.ReadWrite.All_ | Schreib-/Lesezugriff auf alle Gruppen|