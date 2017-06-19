# <a name="user-resource-type"></a>user-Ressourcentyp

Stellt ein Azure AD-Benutzerkonto dar. Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md).
- Verwenden einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/user_delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Benutzer auflisten](../api/user_list.md) |[Benutzersammlung](user.md)| Dient zum Abrufen einer Liste von Benutzerobjekten.|
|[Benutzer erstellen](../api/user_post_users.md) |[Benutzer](user.md)| Dient zum Erstellen eines neuen Benutzerobjekts.|
|[Benutzer abrufen](../api/user_get.md) | [user](user.md) |Liest Eigenschaften und Beziehungen des Benutzerobjekts.|
|[Update user](../api/user_update.md) | [user](user.md) |Aktualisiert das Benutzerobjekt. |
|[Delete user](../api/user_delete.md) | None |Löscht das Benutzerobjekt. |
|[List messages](../api/user_list_messages.md) |[Message](message.md) collection| Ruft alle Nachrichten im Postfach des angemeldeten Benutzers ab.|
|[Create Message](../api/user_post_messages.md) |[Message](message.md)| Erstellt eine neue Nachricht durch Veröffentlichung in der Nachrichtensammlung.|
|[List mailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) collection| Ruft die E-Mail-Ordner-Sammlung unter dem Stammordner des angemeldeten Benutzers ab. |
|[Create mailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Erstellt einen neuen MailFolder durch Veröffentlichung in der mailFolders-Sammlung.|
|[sendMail](../api/user_sendmail.md)|None|Sendet die im Anforderungstext angegebene Nachricht.|
|[List events](../api/user_list_events.md) |[Event](event.md) collection| Ruft eine Liste der event-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Create event](../api/user_post_events.md) |[Event](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Ereignissammlung.|
|[List calendars](../api/user_list_calendars.md) |[Calendar](calendar.md) collection| Ruft eine Kalenderobjektsammlung ab.|
|[Create calendar](../api/user_post_calendars.md) |[Calendar](calendar.md)| Erstellt einen neuen Kalender durch Veröffentlichung in der Kalendersammlung.|
|[List calendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) collection| Ruft eine CalendarGroup-Objektsammlung ab.|
|[Create calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Erstellt eine neue CalendarGroup durch Veröffentlichung in der CalendarGroups-Sammlung.|
|[List calendarView](../api/user_list_calendarview.md) |[Event](event.md) collection| Ruft eine Ereignisobjektsammlung ab.|
|[List contacts](../api/user_list_contacts.md) |[Contact](contact.md) collection| Ruft eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create Contact](../api/user_post_contacts.md) |[Kontakt](contact.md)| Erstellt einen neuen Kontakt durch Veröffentlichung in der Kontaktsesammlung.|
|[List contactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) collection| Ruft die Kontaktordnersammlung im Standardkontaktordner des angemeldeten Benutzers ab.|
|[Create ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Erstellt einen neuen ContactFolder durch Veröffentlichung in der ContactFolders-Sammlung.|
|[List directReports](../api/user_list_directreports.md) |[directoryObject](directoryobject.md) collection| Ruft die Benutzer und Kontakte, die an den Benutzer berichten, aus der directReports-Navigationseigenschaft ab.|
|[List manager](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | Ruft den Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist, aus der manager-Navigationseigenschaft ab.|
|[List memberOf](../api/user_list_memberof.md) |[directoryObject](directoryobject.md) collection| Ruft die Gruppen und Verzeichnisrollen, bei denen dieser Benutzer direktes Mitglied ist, aus der memberOf-Navigationseigenschaft ab.|
|[List ownedDevices](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md) collection| Ruft die Geräte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[List ownedObjects](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[List registeredDevices](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md) collection| Ruft die Geräte, die für den Benutzer registriert sind, aus der registeredDevices-Navigationseigenschaft ab.|
|[List createdObjects](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md) collection| Ruft die Verzeichnisobjekte, die von dem Benutzer erstellt wurden, aus der createdObjects-Navigationseigenschaft ab.|
|[assignLicense](../api/user_assignlicense.md)|[user](user.md)|Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.|
|[licenseDetails auflisten](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md)-Sammlung| Dient zum Abrufen einer licenseDetails-Objektsammlung.| 
|[checkMemberGroups](../api/user_checkmembergroups.md)|String collection|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[getMemberGroups](../api/user_getmembergroups.md)|String collection|Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/user_getmemberobjects.md)|String collection| Gibt alle Gruppen und Verzeichnisrollen zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv. |
|[reminderView](../api/user_reminderview.md)|[Reminder](reminder.md) collection|Gibt eine Liste von Kalendererinnerungen innerhalb der angegebenen Start- und Endzeiten zurück.|
|[delta](../api/user_delta.md)|Benutzersammlung| Dient zum Abrufen inkrementeller Änderungen für Benutzer. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|



## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|aboutMe|String|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|birthday|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|businessPhones|String-Sammlung|Die Telefonnummern für den Benutzer. HINWEIS: Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.|
|Ort|String|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|companyName|String|Der Unternehmensname, dem der Benutzer zugewiesen ist.|
|country|String|Land/Region, in dem/der sich der Benutzer befindet; z. B. „USA“ oder „UK“. Unterstützt $filter.|
|department
|String|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|String|cDer Name, der im Adressbuch für den Benutzer angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $Filter und $orderby.|
|givenName|String|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|String|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|imAddresses|String-Sammlung|Die VOIP-SIP-Adressen (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.|
|interests|String collection|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|String|Die Position des Benutzers. Unterstützt $filter.|
|Mail|String|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Einstellungen für das primäre Postfach des angemeldeten Benutzers. Sie können Einstellungen für das Senden von automatischen Antworten auf eingehende Nachrichten, das Gebietsschema und die Zeitzone [abrufen](../api/user_get_mailboxsettings.md) oder [aktualisieren](../api/user_update_mailboxsettings.md).|
|mailNickname|String|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|String|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|String|Die URL für die persönliche Website des Benutzers.|
|officeLocation|String|Der Bürostandort der Firma des Benutzers|
|onPremisesImmutableId|String|Diese Eigenschaft wird verwendet, um ein lokales Active Directory-Benutzerkonto dem Azure AD-Benutzerobjekt zuzuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto in Graph erstellt wird, wenn Sie eine Verbunddomäne für die **UserPrincipalName**-Eigenschaft (UPN) des Benutzers verwenden. **Wichtig:** Die Zeichen **$** und **_** können nicht verwendet werden, wenn Sie diese Eigenschaft angeben. Unterstützt $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den letzten Zeitpunkt an, zu dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Beispiel: „2013-02-16T03:04:54Z“. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|onPremisesSecurityIdentifier|String|Enthält die lokale Sicherheits-ID (SID) für den Benutzer, der von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt.|
|onPremisesSyncEnabled|Boolean| **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt |
|passwordPolicies|String|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|String collection|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|String|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredLanguage|String|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|String|Der bevorzugte Name für den Benutzer.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|proxyAddresses|String collection|Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Schreibgeschützt, lässt keine NULL-Werte zu. Unterstützt $filter.          |
|responsibilities|String collection|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|schools|String collection|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|skills|String collection|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|state|String|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|String|Die Straße der Firma des Benutzers.|
|surname|String|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|String|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|String|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|String|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|calendar|[Calendar](calendar.md)|Primärer Kalender des Benutzers. Schreibgeschützt.|
|calendarGroups|[CalendarGroup](calendargroup.md) collection|Die Kalendergruppen des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendarView|[Event](event.md) collection|Die Kalenderansicht für den Kalender. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendars|[Calendar](calendar.md) collection|Die Kalender des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contactFolders|[ContactFolder](contactfolder.md) collection|Die Kontakteordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contacts|[Contact](contact.md) collection|Die Kontakte des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|createdObjects|[directoryObject](directoryobject.md) collection|Verzeichnisobjekte, die vom Benutzer erstellt wurden. Schreibgeschützt. Lässt NULL-Werte zu.|
|directReports|[directoryObject](directoryobject.md) collection|Die Benutzer und Kontakte, die an den Benutzer berichten. (Die Benutzer und Kontakte, deren manager-Eigenschaft auf diesen Benutzer festgelegt ist.) Schreibgeschützt. Lässt NULL-Werte zu. |
|drive|[drive](drive.md)|OneDrive eines Benutzers. Schreibgeschützt.|
|drives|[drive](drive.md)-Sammlung. | Eine Sammlung von Laufwerken, die für diesen Benutzer zur Verfügung stehen. Schreibgeschützt. |
|events|[Event](event.md) collection|Die Ereignisse des Benutzers. Standardmäßig werden Ereignisse unter dem Standard-Kalender angezeigt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für den Benutzer definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | Relevanzklassifizierung von Nachrichten des Benutzers basierend auf expliziten Kennzeichnungen, die die abgeleitete Relevanz oder Wichtigkeit außer Kraft setzen. |
|mailFolders|[MailFolder](mailfolder.md) collection| Die E-Mail-Ordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|manager|[directoryObject](directoryobject.md)|Der Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist. Schreibgeschützt. (HTTP-Methoden: GET, PUT, DELETE.)|
|memberOf|[directoryObject](directoryobject.md) collection|Die Gruppen und Verzeichnisrollen, bei denen der Benutzer Mitglied ist. Schreibgeschützt. Lässt NULL-Werte zu.|
|messages|[Message](message.md) collection|Die Nachrichten in einem Postfach oder Ordner. Schreibgeschützt. Lässt NULL-Werte zu.|
|onenote|[OneNote](onenote.md)| Schreibgeschützt.|
|ownedDevices|[directoryObject](directoryobject.md) collection|Geräte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Verzeichnisobjekte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto des Benutzers. Schreibgeschützt.|
|registeredDevices|[directoryObject](directoryobject.md) collection|Geräte, die für den Benutzer registriert sind. Schreibgeschützt. Lässt Nullwerte zu.|

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
    "messages",
    "oauth2PermissionGrants",
    "onenote",
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
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
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
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
