---
title: user-Ressourcentyp
description: Stellt ein Azure AD-Benutzerkonto dar. Erbt von directoryObject.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9d3ca1c6f9c67cc2e41907dc22b9f1ec7d28b0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972649"
---
# <a name="user-resource-type"></a>user-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein Azure AD-Benutzerkonto dar. Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).
- Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
|[Benutzer auflisten](../api/user-list.md) |[Benutzersammlung](user.md)| Dient zum Abrufen einer Liste von Benutzerobjekten.|
|[Benutzer erstellen](../api/user-post-users.md) |[Benutzer](user.md)| Dient zum Erstellen eines neuen Benutzerobjekts.|
|[Benutzer abrufen](../api/user-get.md) | [user](user.md) |Liest Eigenschaften und Beziehungen des Benutzerobjekts.|
|[Update user](../api/user-update.md) | [user](user.md) |Aktualisiert das Benutzerobjekt. |
|[Delete user](../api/user-delete.md) | None |Löscht das Benutzerobjekt. |
|[List messages](../api/user-list-messages.md) |[Message](message.md) collection| Ruft alle Nachrichten im Postfach des angemeldeten Benutzers ab.|
|[Create Message](../api/user-post-messages.md) |[Nachricht](message.md)| Erstellen Sie eine Nachricht, durch die Veröffentlichung auf der Nachrichten-Auflistung.|
|[List mailFolders](../api/user-list-mailfolders.md) |[MailFolder](mailfolder.md) collection| Ruft die E-Mail-Ordner-Sammlung unter dem Stammordner des angemeldeten Benutzers ab. |
|[Create mailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| Erstellt einen neuen MailFolder durch Veröffentlichung in der mailFolders-Sammlung.|
|[sendMail](../api/user-sendmail.md)|None|Sendet die im Anforderungstext angegebene Nachricht.|
|[List events](../api/user-list-events.md) |[Event](event.md) collection| Ruft eine Liste der event-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Ereignis erstellen](../api/user-post-events.md) |[Event](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Ereignissammlung.|
|[List calendars](../api/user-list-calendars.md) |[Calendar](calendar.md) collection| Ruft eine Kalenderobjektsammlung ab.|
|[Create calendar](../api/user-post-calendars.md) |[Calendar](calendar.md)| Erstellt einen neuen Kalender durch Veröffentlichung in der Kalendersammlung.|
|[List calendarGroups](../api/user-list-calendargroups.md) |[CalendarGroup](calendargroup.md) collection| Ruft eine CalendarGroup-Objektsammlung ab.|
|[Create calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Erstellt eine neue CalendarGroup durch Veröffentlichung in der CalendarGroups-Sammlung.|
|[List calendarView](../api/user-list-calendarview.md) |[Event](event.md) collection| Get-Auflistung ein Event-Objekts.|
|[List contacts](../api/user-list-contacts.md) |[Contact](contact.md) collection| Ruft eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create Contact](../api/user-post-contacts.md) |[Kontakt](contact.md)| Erstellt einen neuen Kontakt durch Veröffentlichung in der Kontaktsesammlung.|
|[List contactFolders](../api/user-list-contactfolders.md) |[ContactFolder](contactfolder.md) collection| Ruft die Kontaktordnersammlung im Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| Erstellt einen neuen ContactFolder durch Veröffentlichung in der ContactFolders-Sammlung.|
|[List directReports](../api/user-list-directreports.md) |[directoryObject](directoryobject.md) collection| Ruft die Benutzer und Kontakte, die an den Benutzer berichten, aus der directReports-Navigationseigenschaft ab.|
|[List manager](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Ruft den Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist, aus der manager-Navigationseigenschaft ab.|
|[List memberOf](../api/user-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie die Gruppen, Directory Rollen und administrative Einheiten, die der Benutzer ein direktes Mitglied in der Navigationseigenschaft Mitglied ist.|
|[Transitive Mitglied Liste](../api/user-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Auflisten der Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist. Dieser Vorgang ist transitiv und enthält die Gruppen, denen der Benutzer ein geschachtelte Mitglied ist. |
|[joinedTeams auflisten](../api/user-list-joinedteams.md) |[Groups](group.md) -Auflistung| Rufen Sie die Microsoft-Teams, dass der Benutzer ein direktes Mitglied in der Navigationseigenschaft JoinedTeams ist.|
|[List ownedDevices](../api/user-list-owneddevices.md) |[directoryObject](directoryobject.md) collection| Ruft die Geräte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[List ownedObjects](../api/user-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[plannerTasks auflisten](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md)-Sammlung| Möchten Sie dem Benutzer zugewiesene PlannerTasks erhalten.|
|[List registeredDevices](../api/user-list-registereddevices.md) |[directoryObject](directoryobject.md) collection| Rufen Sie die Geräte, die registriert sind, für den Benutzer aus der RegisteredDevices Navigation-Eigenschaft.|
|[Mitgliedschaften bezogenen-Rolle](../api/user-list-scopedrolememberof.md) |[scopedRoleMembership](scopedrolemembership.md)-Sammlung| Abrufen der bezogenen Rolle administrative Einheiten Mitgliedschaften für diesen Benutzer.|
|[List createdObjects](../api/user-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die von dem Benutzer erstellt wurden, aus der createdObjects-Navigationseigenschaft ab.|
|[Liste agreementAcceptances](../api/user-list-agreementacceptances.md) | [AgreementAcceptance](agreementacceptance.md) -Auflistung | Rufen Sie eine Liste der rechtliche Hinweise Annahme Status des Benutzers.|
|[assignLicense](../api/user-assignlicense.md)|[Benutzer](user.md)|Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.|
|[licenseDetails auflisten](../api/user-list-licensedetails.md) |[licenseDetails](licensedetails.md)-Sammlung| Dient zum Abrufen einer licenseDetails-Objektsammlung.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|Zeichenfolgenauflistung|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[findmeetingtimes](../api/user-findmeetingtimes.md)|[meetingTimeCandidate](meetingtimecandidate.md)|Hier finden Sie Zeit und Speicherorte basierend auf der Verfügbarkeit erfüllen, Standort oder Zeit Einschränkungen.|
|[findRoomLists](../api/user-findroomlists.md)|[EmailAddress.MD](emailaddress.md) -Auflistung | Abrufen von Raumlisten in einem Mandanten definiert.|
|[findRooms](../api/user-findrooms.md)|[EmailAddress.MD](emailaddress.md) -Auflistung | Rufen Sie allen Besprechungsräumen Mandant des Benutzers oder in einer bestimmten Raumliste. |
|[getMailTips](../api/user-getmailtips.md)|[mailTips](mailtips.md)-Sammlung|Geben Sie die MailTips für einen oder mehrere Empfänger als verfügbar für den angemeldeten Benutzer zurück. |
|[getMemberGroups](../api/user-getmembergroups.md)|Zeichenfolgenauflistung|Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Zeichenfolgenauflistung| Zurückgeben Sie aller Gruppen, Directory Rollen und administrative Einheiten, denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv. |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| Keine |Ungültig des Benutzers Aktualisierung und Sitzung ausgestellten Token als für Clientanwendungen, indem Sie auf das aktuelle Datum-Uhrzeit die Benutzereigenschaft **RefreshTokensValidFromDateTime** zurücksetzen. Dies erzwingt, dass den Benutzer mit diesen Anwendungen erneut anmelden.|
|[reminderView](../api/user-reminderview.md)|[Reminder](reminder.md) collection|Gibt eine Liste von Kalendererinnerungen innerhalb der angegebenen Start- und Endzeiten zurück.|
|[delta](../api/user-delta.md)|Benutzersammlung| Dient zum Abrufen inkrementeller Änderungen für Benutzer. |
|[Übersetzen von Outlook-IDs](../api/user-translateexchangeids.md) |[Ressourcentyp ConvertIdResult](convertidresult.md) -Auflistung| Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    | Beschreibung |
|:---------------|:--------|:------------|
|aboutMe|Zeichenfolge|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|ageGroup|Zeichenfolge|Die ALTER Gruppe des Benutzers festgelegt. Zulässige Werte: `null`, `minor`, `notAdult` und `adult`. Die [rechtliche Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen finden Sie unter. |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|assignedPlans|[assignedPlan](assignedplan.md)-Sammlung|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|birthday|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|city|Zeichenfolge|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|companyName| String | Der Unternehmensname, dem der Benutzer zugewiesen ist. Schreibgeschützt.
|consentProvidedForMinor|Zeichenfolge|Legt fest, ob Zustimmung für Minderjährige abgerufen wurde. Zulässige Werte: `null`, `granted`, `denied` und `notRequired`. Die [rechtliche Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen finden Sie unter.|
|Land|Zeichenfolge|Das Land/Region, in dem sich der Benutzer befindet; "USA" oder "UK". Unterstützt $filter.|
|deletedDateTime|DateTimeOffset| Das Datum und die Zeit, die der Benutzer gelöscht wurde. |
|department|Zeichenfolge|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|Zeichenfolge|Der Name des Benutzers, der im Adressbuch angezeigt wird. Dieser Wert ist in der Regel die Kombination aus den Vornamen des Benutzers, mittleren ersten und letzten Namen. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $filter und $orderby.|
|employeeId|Zeichenfolge|Die Mitarbeiter-ID von der Organisation, die dem Benutzer zugewiesen. Unterstützt $filter.|
|externalUserState|Zeichenfolge|Für einen externen Benutzer eingeladen, den Mandanten mit der [Einladung API](../api/invitation-post.md)stellt diese Eigenschaft die eingeladene Benutzer Einladungsstatus. Für eingeladene Benutzer kann der Status 'PendingAcceptance' oder 'Akzeptiert' sein oder `null` für alle anderen Benutzer. Unterstützt $filter mit unterstützten Werte. Zum Beispiel: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|Zeichenfolge|Zeigt den Zeitstempel für die letzte Änderung der ExternalUserState-Eigenschaft.|
|Faxnummer|Zeichenfolge|Die Faxnummer des Benutzers.|
|givenName|Zeichenfolge|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|String|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|interests|Zeichenfolgenauflistung|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|Zeichenfolge|Die Position des Benutzers. Unterstützt $filter.|
|legalAgeGroupClassification|Zeichenfolge| Wird von enterpriseanwendungen verwendet, um der Altersgruppe Legal des Benutzers zu bestimmen. Diese Eigenschaft ist schreibgeschützt und berechnete basierend auf `ageGroup` und `consentProvidedForMinor` Eigenschaften. Zulässige Werte: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` und `adult`. Verweisen Sie auf die [Legal Alter mitgliedergruppendefinitionen-Eigenschaft](#legal-age-group-property-definitions) für Weitere Informationen.)|
|licenseAssignmentStates|[LicenseAssignmentState](licenseassignmentstate.md) -Auflistung|Status der Lizenz Zuordnungen für diesen Benutzer. Schreibgeschützt.|
|mail|Zeichenfolge|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Einstellungen für das primäre Postfach des angemeldeten Benutzers. Sie können [Abrufen](../api/user-get-mailboxsettings.md) oder [Aktualisieren von](../api/user-update-mailboxsettings.md) Einstellungen für automatische Antworten auf eingehende Nachrichten, Gebietsschema und Zeitzone senden.|
|mailNickname|Zeichenfolge|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|Zeichenfolge|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|Zeichenfolge|Die URL für die persönliche Website des Benutzers.|
|officeLocation|Zeichenfolge|Der Bürostandort der Firma des Benutzers|
|onPremisesDistinguishedName|Zeichenfolge| Enthält das lokale Active Directory `distinguished name` oder `DN`. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|onPremisesDomainName|Zeichenfolge| Enthält lokale `domainFQDN`, auch als bezeichnet DnsDomänenName aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|"Extensionattributes" 1-15 für den Benutzer enthält. Beachten Sie, dass der einzelnen Erweiterungsattribute auswählbar weder gefiltert werden. Für eine `onPremisesSyncEnabled` Benutzer, diese Gruppe von Eigenschaften ist dem Format mastered lokale und ist schreibgeschützt. Für einen Benutzer nur-Cloud-(wobei `onPremisesSyncEnabled` ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren. |
|onPremisesImmutableId|Zeichenfolge|Diese Eigenschaft wird verwendet, um eine lokale Active Directory-Benutzerkonto in ihrer Azure AD-Benutzerobjekt zuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto im Diagramm zu erstellen, wenn Sie für des Benutzers eine verbunddomäne verwenden `userPrincipalName` -Eigenschaft (UPN). **Wichtig:** Die **$** **_** Zeichen verwendet werden, wenn Sie diese Eigenschaft festlegen. Unterstützt $filter. |
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den letzten Zeitpunkt an, zu dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Beispiel: „2013-02-16T03:04:54Z“. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|onPremisesProvisioningErrors|[OnPremisesProvisioningError](onpremisesprovisioningerror.md) -Auflistung| Fehler beim Microsoft Synchronisierung während der Bereitstellung verwenden. |
|onPremisesSamAccountName|Zeichenfolge| Enthält lokale `sAMAccountName` aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|onPremisesSecurityIdentifier|Zeichenfolge|Enthält die lokale Sicherheits-ID (SID) für den Benutzer, der von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt.|
|onPremisesSyncEnabled|Boolean| **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt |
|onPremisesUserPrincipalName|Zeichenfolge| Enthält lokale `userPrincipalName` aus dem lokalen Verzeichnis synchronisiert. Die Eigenschaft wird nur für Kunden aufgefüllt, die ihre lokalen Verzeichnis zu Azure Active Directory über Azure AD-Connect synchronisiert werden. Schreibgeschützt. |
|otherMails|Zeichenfolge| Eine Liste der weitere e-Mail-Adressen für den Benutzer; Beispiel: `["bob@contoso.com", "Robert@fabrikam.com"]`. Unterstützt $filter.|
|passwordPolicies|Zeichenfolge|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|Zeichenfolge|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredDataLocation|Zeichenfolge|Die bevorzugte Datenspeicherort für den Benutzer. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|Zeichenfolge|Der bevorzugte Name für den Benutzer.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|proxyAddresses|Zeichenfolgenauflistung|Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Schreibgeschützt, lässt keine NULL-Werte zu. Unterstützt $filter.          |
|refreshTokensValidFromDateTime|DateTimeOffset| Eine beliebige Aktualisierungstoken oder Sitzungen Token (Sitzungscookies) ausgestellt vor diesem Zeitpunkt sind ungültig und Applikationen erhalten eine Fehlermeldung, wenn ein ungültiger Aktualisierungs- oder Sitzungen Token verwenden, um ein delegierter Zugriff zu erwerben token (um beispielsweise Microsoft Graph APIs zugreifen).  In diesem Fall müssen die Anwendung ein neues Aktualisierungstoken erhalten, indem er eine Anforderung an den Endpunkt autorisieren. Schreibgeschützt. Verwenden Sie [InvalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) zurücksetzen.|
|responsibilities|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|schools|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|showInAddressList|Boolescher Wert|**true,** Wenn die globalen Adressliste von Outlook, diese Benutzer, andernfalls **false enthalten soll**. Wenn kein Wert festgelegt, dies als **true**behandelt wird. Für Benutzer, die über die Einladung Manager eingeladen wird diese Eigenschaft auf **false**festgelegt.|
|skills|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|state|Zeichenfolge|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|Zeichenfolge|Die Straße der Firma des Benutzers.|
|surname|Zeichenfolge|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|Zeichenfolge|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|String|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|Zeichenfolge|Ein String-Wert, der zum Klassifizieren Benutzertypen in Ihrem Verzeichnis, beispielsweise "Members" und "Gast" verwendet werden kann. Unterstützt $filter.          |

### <a name="legal-age-group-property-definitions"></a>Legal Alter mitgliedergruppendefinitionen-Eigenschaft

In diesem Abschnitt wird erläutert, wie die drei Gruppeneigenschaften Alter (`legalAgeGroupClassification`, `ageGroup` und `consentProvidedForMinor`) werden von Azure AD-Administratoren und Anwendungsentwickler Enterprise verwendet, um die ALTER-bezogene Auflagen erfüllen.

Beispiel: Cameron ist Administrator eines Verzeichnisses für eine Grundschule in Holyport im Vereinigten Königreich. Am Anfang des Jahres School wird er die Aufnahmen Unterlagen Zustimmung von der Minor übergeordneten Elementen basierend auf den Alter-bezogene Vorschriften der im Vereinigten Königreich abgerufen. Die Zustimmung des übergeordneten Objekts kann die Nebenversionsnummer Konto von Holyport Schule und Microsoft apps verwendet werden. Cameron klicken Sie dann alle Konten erstellt und AgeGroup auf "minor" und "erteilt" ConsentProvidedForMinor festgelegt. Durch seinen Studenten verwendete Anwendungen können dann Features zu unterdrücken, die nicht für Minderjährige geeignet sind.

#### <a name="legal-age-group-classification"></a>Legal Alter Gruppe Klassifikation

Diese Eigenschaft schreibgeschützt wird von Enterprise-Anwendungsentwickler verwendet, um sicherzustellen, dass die richtige Handhabung eines Benutzers basierend auf ihrer Legal Altersgruppe. Es wird berechnet, basierend auf dem Benutzer `ageGroup` und `consentProvidedForMinor` Eigenschaften.

| Wert   | # |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `ageGroup` für den Benutzer festgelegt wurde.|
|minorWithoutParentalConsent |1|(Für die zukünftige Verwendung reserviert)|
|minorWithParentalConsent|2| Der Benutzer ist ein Minor basierend auf dem Alter-bezogene Vorschriften ihres Landes betrachtet oder Region und der Administrator des Kontos aus Erziehungsberechtigte entsprechende Zustimmung erhalten hat.|
|oben|3|Der Benutzer betrachtet basierend auf der ALTER-bezogene Vorschriften ihrer Land oder Region oben.|
|notAdult|4|Der Benutzer hat ihren Ursprung einem Land oder Region, die zusätzliche Alter-bezogene Vorschriften (beispielsweise USA, Vereinigtes Königreich, Europäische Union oder South Korea) verfügt, und das Alter des Benutzers ist zwischen einem Minor und ein Versender nicht jugendfreier Alter (als vorgesehenen basierend auf Land oder Region). Im Allgemeinen, dies bedeutet, dass Teenager als gelten `notAdult` in regulierten Ländern.|
|minorNoParentalConsentRequired|5|Der Benutzer ist ein Minor aber aus einem Land oder Region, die keine Vorschriften Alter-bezogene hat.|

#### <a name="age-group-and-minor-consent"></a>Alter Gruppe und minor Zustimmung

Die ALTER Gruppe und minor Zustimmung sind optionalen Eigenschaften von Azure AD-Administratoren verwendet, um sicherzustellen, dass die Verwendung eines Kontos ordnungsgemäß basierend auf der ALTER-bezogene behördlichen Vorschriften für Land oder Region des Benutzers behandelt wird.

#### <a name="agegroup-property"></a>AgeGroup-Eigenschaft

| Wert    | # |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `ageGroup` für den Benutzer festgelegt wurde.|
|minor|1|Der Benutzer ist ein Minor berücksichtigen.|
|notAdult|2|Der Benutzer ist aus einem Land, die gesetzliche Vorschriften, USA, Vereinigtes Königreich, Europäische Union oder South Korea hat) und Alter des Benutzers ist größer als die obere Grenze der Kind Alter (gemäß den Anweisungen in Land) und weniger als untere Grenze der Versender nicht jugendfreier Alter (als vorgesehenen basierend auf Land oder Region) . Teenager praktisch, gelten als `notAdult` in regulierten Ländern.|
|oben|3|Der Benutzer sollte wie oben behandelten sein.|

#### <a name="consentprovidedforminor-property"></a>ConsentProvidedForMinor-Eigenschaft

| Wert    | # |Beschreibung|
|:---------------|:--------|:----------|
|null|0|Standardwert nicht `consentProvidedForMinor` für den Benutzer festgelegt wurde.|
|erteilt|1|Der Benutzer über ein Konto verfügen hat Einwilligung wurde.|
|denied|2|Zustimmung wurde nicht für den Benutzer ein Konto abgerufen wurden.|
|notRequired|3|Der Benutzer ist an einem Standort, der keine Zustimmung erforderlich ist.|

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|agreementAcceptances|[AgreementAcceptance](agreementacceptance.md) -Auflistung| Der Benutzer Begriffe der Verwendung Annahme Status. Schreibgeschützt. Lässt Nullwerte zu.|
|Kalender|[Kalender](calendar.md)|Primärer Kalender des Benutzers. Schreibgeschützt.|
|calendarGroups|[CalendarGroup](calendargroup.md) -Auflistung|Die Kalendergruppen des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendarView|[Ereignissammlung](event.md)|Die Kalenderansicht für den Kalender. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendars|[calender](calendar.md)-Sammlung|Die Kalender des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contactFolders|[ContactFolder](contactfolder.md) -Auflistung|Die Kontakteordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contacts|[contact](contact.md)-Sammlung|Die Kontakte des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|createdObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die vom Benutzer erstellt wurden. Schreibgeschützt. Lässt NULL-Werte zu.|
|directReports|[directoryObject](directoryobject.md) collection|Die Benutzer und Kontakte, die an den Benutzer berichten. (Die Benutzer und Kontakte, deren manager-Eigenschaft auf diesen Benutzer festgelegt ist.) Schreibgeschützt. Lässt NULL-Werte zu. |
|drive|[drive](drive.md)|OneDrive eines Benutzers. Schreibgeschützt.|
|events|[Ereignissammlung](event.md)|Die Ereignisse des Benutzers. Standardmäßig werden Ereignisse unter dem Standard-Kalender angezeigt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Auflistung der open-Erweiterungen für den Benutzer definiert. Lässt Nullwerte zu.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Relevanzklassifizierung von Nachrichten des Benutzers basierend auf expliziten Kennzeichnungen, die die abgeleitete Relevanz oder Wichtigkeit außer Kraft setzen. |
|Einblicke in die|[Insights](insights.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|
|joinedGroups|[Gruppensammlung](group.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|mailFolders|[mailFolder](mailfolder.md)-Sammlung| Die E-Mail-Ordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|manager|[directoryObject](directoryobject.md)|Der Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist. Schreibgeschützt. (HTTP-Methoden: GET, PUT, DELETE.)|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Die Gruppen, Verzeichnisrollen und administrativen Einheiten, bei denen der Benutzer ein Mitglied ist. Schreibgeschützt. Lässt NULL-Werte zu.|
|joinedTeams|[Gruppensammlung](group.md)|Die Microsoft-Teams, denen der Benutzer Mitglied ist. Schreibgeschützt. Lässt Nullwerte zu.|
|Nachrichten|[message](message.md)-Sammlung|Die Nachrichten in einem Postfach oder Ordner. Schreibgeschützt. Lässt NULL-Werte zu.|
|onenote|[OneNote](onenote.md)| Schreibgeschützt.|
|Outlook|[outlookUser](outlookuser.md)| Selektive Outlook-Dienste für den Benutzer verfügbar. Schreibgeschützt. Lässt Nullwerte zu.|
|ownedDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|ownedObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Personen|[Person](person.md) -Auflistung| Schreibgeschützt. Die wichtigsten Personen für den Benutzer. Die Sammlung ist nach ihrer Relevanz für den Benutzer sortiert, die von der Kommunikation, der Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt. Eine Person ist eine Ansammlung von Informationen aus E-Mails, Kontakten und sozialen Netzwerken.|
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto des Benutzers. Schreibgeschützt.|
|Fotos|[photo](photo.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|Planner|[plannerUser](planneruser.md)| Selektive Planner-Dienste für den Benutzer zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu. |
|sharepoint|[sharepoint](sharepoint.md)| Zugriff auf die SharePoint-Website des Benutzers. Schreibgeschützt. |
|scopedRoleMemberOf|[scopedRoleMembership](scopedrolemembership.md)-Sammlung| Die administrative Einheit bezogenen Rolle Mitgliedschaften für diesen Benutzer. Schreibgeschützt. Lässt Nullwerte zu.|
|settings|[Settings](user-settings.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|
|registeredDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die für den Benutzer registriert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "insights": { "@odata.type": "microsoft.graph.officeGraphInsights" },
  "settings": { "@odata.type": "microsoft.graph.userSettings" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "joinedTeams": [ { "@odata.type": "microsoft.graph.group" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
