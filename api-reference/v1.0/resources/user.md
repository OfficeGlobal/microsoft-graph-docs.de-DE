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
|[Benutzer abrufen](../api/user_get.md) | [Benutzer](user.md) |Liest Eigenschaften und Beziehungen des Benutzerobjekts.|
|[Benutzer aktualisieren](../api/user_update.md) | [Benutzer](user.md) |Aktualisiert das Benutzerobjekt. |
|[Benutzer löschen](../api/user_delete.md) | Keine |Löscht das Benutzerobjekt. |
|[Nachrichten-Liste](../api/user_list_messages.md) |[Nachrichten](message.md)-Sammlung| Ruft alle Nachrichten im Postfach des angemeldeten Benutzers ab.|
|[Nachricht erstellen](../api/user_post_messages.md) |[Nachricht](message.md)| Erstellt eine neue Nachricht durch Veröffentlichung in der Nachrichtensammlung.|
|[Liste mailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md)-Sammlung| Ruft die E-Mail-Ordner-Sammlung unter dem Stammordner des angemeldeten Benutzers ab. |
|[mailFolder erstellen](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Erstellt einen neuen MailFolder durch Veröffentlichung in der mailFolders-Sammlung.|
|[sendMail](../api/user_sendmail.md)|Keine|Sendet die im Anforderungstext angegebene Nachricht.|
|[Liste der Ereignisse](../api/user_list_events.md) |[Ereignis](event.md)-Sammlung| Ruft eine Liste der event-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Ereignis erstellen](../api/user_post_events.md) |[Ereignis](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Ereignissammlung.|
|[Liste der Kalender](../api/user_list_calendars.md) |[Kalender](calendar.md)-Sammlung| Ruft eine Kalenderobjektsammlung ab.|
|[Kalender erstellen](../api/user_post_calendars.md) |[Kalender](calendar.md)| Erstellt einen neuen Kalender durch Veröffentlichung in der Kalendersammlung.|
|[Liste calendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md)-Sammlung| Ruft eine CalendarGroup-Objektsammlung ab.|
|[calendarGroup erstellen](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Erstellt eine neue CalendarGroup durch Veröffentlichung in der CalendarGroups-Sammlung.|
|[Liste calendarView](../api/user_list_calendarview.md) |[Ereignis](event.md)-Sammlung| Ruft eine Ereignisobjektsammlung ab.|
|[Liste Kontakte](../api/user_list_contacts.md) |[Kontakte](contact.md)-Sammlung| Ruft eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers ab.|
|[Kontakt erstellen](../api/user_post_contacts.md) |[Kontakt](contact.md)| Erstellt einen neuen Kontakt durch Veröffentlichung in der Kontaktsesammlung.|
|[Liste contactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md)-Sammlung| Ruft die Kontaktordnersammlung im Standardkontaktordner des angemeldeten Benutzers ab.|
|[Erstellen ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Erstellt einen neuen ContactFolder durch Veröffentlichung in der ContactFolders-Sammlung.|
|[Liste directReports](../api/user_list_directreports.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer und Kontakte, die an den Benutzer berichten, aus der directReports-Navigationseigenschaft ab.|
|[Listen-Manager](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | Ruft den Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist, aus der manager-Navigationseigenschaft ab.|
|[Liste memberOf](../api/user_list_memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Gruppen und Verzeichnisrollen, bei denen dieser Benutzer direktes Mitglied ist, aus der memberOf-Navigationseigenschaft ab.|
|[Liste ownedDevices](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Geräte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[Liste ownedObjects](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Verzeichnisobjekte, die dem Benutzer gehören, aus der ownedDevices-Navigationseigenschaft ab.|
|[Liste registeredDevices](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Geräte, die für den Benutzer registriert sind, aus der registeredDevices-Navigationseigenschaft ab.|
|[Liste createdObjects](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Verzeichnisobjekte, die von dem Benutzer erstellt wurden, aus der createdObjects-Navigationseigenschaft ab.|
|[assignLicense](../api/user_assignlicense.md)|[Benutzer](user.md)|Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.|
|[licenseDetails auflisten](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md)-Sammlung| Dient zum Abrufen einer licenseDetails-Objektsammlung.|
|[checkMemberGroups](../api/user_checkmembergroups.md)|Zeichenfolgenauflistung|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[getMemberGroups](../api/user_getmembergroups.md)|Zeichenfolgenauflistung|Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/user_getmemberobjects.md)|Zeichenfolgenauflistung| Gibt alle Gruppen und Verzeichnisrollen zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv. |
|[reminderView](../api/user_reminderview.md)|[Erinnerung](reminder.md)-Sammlung|Gibt eine Liste von Kalendererinnerungen innerhalb der angegebenen Start- und Endzeiten zurück.|
|[Delta](../api/user_delta.md)|Benutzersammlung| Dient zum Abrufen inkrementeller Änderungen für Benutzer. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|aboutMe|Zeichenfolge|Ein Freihandform-Texteingabefeld, in dem der Benutzer sich selbst beschreiben kann.|
|accountEnabled|Boolesch| **wahr**, wenn das Konto aktiviert ist; andernfalls **falsch**. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Unterstützt $filter.    |
|ageGroup|Zeichenfolge|Legt die Altersgruppe der Benutzer fest. Zulässige Werte: `null`, `minor`, `notAdult` und `adult`. Weitere Informationen finden Sie unter [Definitionen zu Eigenschaften der Volljährigkeit](#legal-age-group-property-definitions). |
|assignedLicenses|[assignedLicense](assignedlicense.md)-Sammlung|Die Lizenzen, die dem Benutzer zugewiesen sind. Lässt keine NULL-Werte zu.            |
|assignedPlans|[assignedPlan](assignedplan.md)-Sammlung|Die Pläne, die dem Benutzer zugewiesen sind. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|Geburtsdatum|DateTimeOffset|Der Geburtstag des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|businessPhones|String-Sammlung|Die Telefonnummern für den Benutzer. HINWEIS: Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.|
|Ort|Zeichenfolge|Die Stadt, in der sich der Benutzer befindet. Unterstützt $filter.|
|companyName| Zeichenfolge | Der Unternehmensname, dem der Benutzer zugewiesen ist. Schreibgeschützt.
|consentProvidedForMinor|Zeichenfolge|Legt fest, ob Zustimmung für Minderjährige abgerufen wurde. Zulässige Werte: `null`, `granted`, `denied` und `notRequired`. Weitere Informationen finden Sie unter [Definitionen zu Eigenschaften der Volljährigkeit](#legal-age-group-property-definitions).|
|Land|Zeichenfolge|Land/Region, in dem/der sich der Benutzer befindet; z. B. „USA“ oder „UK“. Unterstützt $filter.|
|Abteilung|Zeichenfolge|Der Name der Abteilung, in der der Benutzer arbeitet. Unterstützt $filter.|
|displayName|Zeichenfolge|cDer Name, der im Adressbuch für den Benutzer angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. Unterstützt $Filter und $orderby.|
|givenName|Zeichenfolge|Der Vorname des Benutzers. Unterstützt $filter.|
|hireDate|DateTimeOffset|Das Einstellungsdatum des Benutzers. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|ID|Zeichenfolge|Der eindeutige Bezeichner des Benutzers. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|imAddresses|String-Sammlung|Die VOIP-SIP-Adressen (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.|
|Interessen|Zeichenfolgenauflistung|Eine Liste für den Benutzer, um dessen Interessen zu beschreiben.|
|jobTitle|Zeichenfolge|Die Position des Benutzers. Unterstützt $filter.|
|legalAgeGroupClassification|Zeichenfolge| Wird von Unternehmensanwendungen verwendet, um die Altersgruppe für die Volljährigkeit zu bestimmen. Diese Eigenschaft ist schreibgeschützt und wurde basierend auf `ageGroup` und `consentProvidedForMinor` Eigenschaften berechnet. Zulässige Werte: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` und `adult`. Weitere Informationen finden Sie unter [Definitionen zu Eigenschaften der Volljährigkeit](#legal-age-group-property-definitions).|
|Mail|Zeichenfolge|Die SMTP-Adresse des Benutzers, z. B. „jeff@contoso.onmicrosoft.com“. Schreibgeschützt. Unterstützt $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Einstellungen für das primäre Postfach des angemeldeten Benutzers. Sie können Einstellungen für das Senden von automatischen Antworten auf eingehende Nachrichten, das Gebietsschema und die Zeitzone [abrufen](../api/user_get_mailboxsettings.md) oder [aktualisieren](../api/user_update_mailboxsettings.md).|
|mailNickname|Zeichenfolge|Der E-Mail-Alias für den Benutzer. Diese Eigenschaft muss beim Erstellen eines Benutzers angegeben werden. Unterstützt $filter.|
|mobilePhone|Zeichenfolge|Die Nummer des primären Mobiltelefons für den Benutzer.|
|mySite|Zeichenfolge|Die URL für die persönliche Website des Benutzers.|
|officeLocation|Zeichenfolge|Der Bürostandort der Firma des Benutzers|
|onPremisesDomainName|Zeichenfolge| Enthält lokale `domainFQDN`, auch dnsDomänenName bezeichnet, die aus dem lokalen Verzeichnis synchronisiert wurden. Die Eigenschaft wird nur für Kunden ausgefüllt, die ihr lokales Verzeichnis mit Azure AD Connect zu Azure Active Directory synchronisieren. Schreibgeschützt. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|Enthält die "Extensionattributes" 1-15 für den Benutzer. Beachten Sie, dass einzelne Erweiterungsattribute weder ausgewählt noch gefiltert werden können. Für einen `onPremisesSyncEnabled`-Benutzer wird diese Eigenschaftengruppe lokal gemastert und ist schreibgeschützt. Für einen Nur-Cloud-Benutzer (wobei `onPremisesSyncEnabled` falsch ist) können diese Eigenschaften während der Erstellung oder der Aktualisierung festgelegt werden. |
|onPremisesImmutableId|Zeichenfolge|Diese Eigenschaft wird verwendet, um ein lokales Active Directory-Benutzerkonto dem Azure AD-Benutzerobjekt zuzuordnen. Diese Eigenschaft muss angegeben werden, wenn ein neues Benutzerkonto in Graph erstellt wird, wenn Sie eine Verbunddomäne für die **UserPrincipalName**-Eigenschaft (UPN) des Benutzers verwenden. **Wichtig:** Die Zeichen **$** und **_** können nicht verwendet werden, wenn Sie diese Eigenschaft angeben. Unterstützt $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt den letzten Zeitpunkt an, zu dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Beispiel: „2013-02-16T03:04:54Z“. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)-Sammlung| Fehler bei der Nutzung des Produkts zur Synchronisierung von Microsoft während Provisioning. |
|onPremisesSamAccountName|Zeichenfolge| Enthält lokale `samAccountName`, die aus dem lokalen Verzeichnis synchronisiert wurden. Die Eigenschaft wird nur für Kunden ausgefüllt, die ihr lokales Verzeichnis mit Azure AD Connect zu Azure Active Directory synchronisieren. Schreibgeschützt. |
|onPremisesSecurityIdentifier|Zeichenfolge|Enthält die lokale Sicherheits-ID (SID) für den Benutzer, der von der lokalen Bereitstellung in der Cloud synchronisiert wurde. Schreibgeschützt.|
|onPremisesSyncEnabled|boolesch| **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt |
|onPremisesUserPrincipalName|Zeichenfolge| Enthält lokale `userPrincipalName`, die aus dem lokalen Verzeichnis synchronisiert wurden. Die Eigenschaft wird nur für Kunden ausgefüllt, die ihr lokales Verzeichnis mit Azure AD Connect zu Azure Active Directory synchronisieren. Schreibgeschützt. |
|passwordPolicies|Zeichenfolge|Gibt die Kennwortrichtlinien für den Benutzer an. Dieser Wert ist eine Enumeration, deren einziger möglicher Wert „DisableStrongPassword“ lautet. Damit können schwächere Kennwörter als in der Standardrichtlinie angegeben festgelegt werden. Auch „DisablePasswordExpiration“ kann angegeben werden. Beide können zusammen angegeben werden, z. B.: „DisablePasswordExpiration, DisableStrongPassword“.|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Gibt das Kennwortprofil für den Benutzer an. Das Profil enthält das Kennwort des Benutzers. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Das Kennwort im Profil muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft angegeben. Standardmäßig ist ein sicheres Kennwort erforderlich.|
|pastProjects|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der erledigten Projekte eines Benutzers.|
|postalCode|Zeichenfolge|Die Postleitzahl für die Postanschrift des Benutzers. Die Postleitzahl ist für das Land/die Region des Benutzers spezifisch. In den USA enthält dieses Attribut den ZIP Code.|
|preferredLanguage|Zeichenfolge|Die bevorzugte Sprache für den Benutzer. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en-US“.|
|preferredName|Zeichenfolge|Der bevorzugte Name für den Benutzer.|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md)-Sammlung|Die Pläne, die für den Benutzer bereitgestellt wurden. Schreibgeschützt. Lässt keine NULL-Werte zu. |
|proxyAddresses|Zeichenfolgenauflistung|Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Schreibgeschützt, lässt keine NULL-Werte zu. Unterstützt $filter.          |
|Verantwortlichkeiten|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Verantwortlichkeiten eines Benutzers.|
|Schulen|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der vom Benutzer besuchten Schulen.|
|Qualifikationen|Zeichenfolgenauflistung|Eine Liste zur Aufzählung der Qualifikationen eines Benutzers.|
|Zustand|Zeichenfolge|Bundesland oder Kanton in der Adresse des Benutzers. Unterstützt $filter.|
|streetAddress|Zeichenfolge|Die Straße der Firma des Benutzers.|
|Nachname|Zeichenfolge|Der Nachname des Benutzers. Unterstützt $filter.|
|usageLocation|Zeichenfolge|Ein aus zwei Buchstaben bestehender Ländercode (ISO-Standard 3166). Erforderlich für Benutzer, denen Lizenzen zugewiesen werden, aufgrund der gesetzlichen Vorschrift, dass die Verfügbarkeit von Diensten in einzelnen Ländern geprüft werden muss.  Beispiele sind: „US“, „JP“ und „GB“. Lässt keine NULL-Werte zu. Unterstützt $filter.|
|userPrincipalName|Zeichenfolge|Der User Principal Name (UPN) des Benutzers. Der UPN ist ein Anmeldename des Benutzers im Internetformat, der auf dem Internetstandard RFC 822 basiert. Gemäß der Konvention sollte er dem E-Mail-Namen des Benutzers zugeordnet sein. Das allgemeine Format lautet „alias@domäne“, wobei „domäne“ in der Sammlung der verifizierten Domänen des Mandanten vorhanden sein muss. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Auf die verifizierten Domänen für den Mandanten kann über die **verifiedDomains** -Eigenschaft von [organization](organization.md) zugegriffen werden. Unterstützt $Filter und $orderby.
|userType|Zeichenfolge|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

### <a name="legal-age-group-property-definitions"></a>Definitionen der Volljährigkeits-Eigenschaften von Gruppen

In diesem Abschnitt wird erläutert, wie die drei Gruppeneigenschaften (`legalAgeGroupClassification`, `ageGroup` und `consentProvidedForMinor`) von Azure AD-Administratoren und Anwendungsentwickler-Unternehmen verwendet werden, um altersbezogene Auflagen zu erfüllen.

Beispiel: Cameron ist Administrator eines Verzeichnisses für eine Grundschule in Holyport, Großbritannien. Am Anfang des Schuljahres verwendet er die Aufnahme-Unterlagen für die Einholung der Zustimmung er Eltern der Minderjährigen, basierend auf den altersbezogenen Vorschriften in Großbritannien. Durch die Zustimmung des Elternteils kann das Konto des Minderjährigen von der Holyport-Schule und den Microsoft-Apps verwendet werden. Cameron erstellt dann alle Konten und stellt die ageGroup auf klicken Sie dann alle Konten erstellt und AgeGroup auf „Minderjährig“ und consentProvided ForMinor auf „erteilt“. Von seinen Schülern verwendete Anwendungen können dann Funktionen unterdrücken, die für Minderjährige nicht geeignet sind.

#### <a name="legal-age-group-classification"></a>Einstufung der gesetzlichen Altersgruppe

Diese schreibgeschützte Eigenschaft wird von Unternehmens-Anwendungsentwicklern verwendet, um sicherzustellen, dass die richtige Handhabung eines Benutzers basierend auf seiner gesetzlichen Altersgruppe gewährleistet ist. Diese wird basierend auf dem Benutzer `ageGroup` und den `consentProvidedForMinor`-Eigenschafen berechnet.

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|keine|0|Standardwert nicht `ageGroup` wurde für den Benutzer festgelegt.|
|minorWithoutParentalConsent |1|(Reserviert für die zukünftige Verwendung)|
|minorWithParentalConsent|2| Der Benutzer ist basierend auf den altersbezogenen Vorschriften ihres Landes oder Region als Minderjährig zu betrachten und der Administrator des Kontos hat von den Erziehungsberechtigten die entsprechende Zustimmung erhalten.|
|Erwachsener|3|Der Benutzer wird basierend auf den altersbezogenen Vorschriften seines Landes als Erwachsener betrachtet.|
|notAdult|4|Der Benutzer hat seinen Ursprung in einem Land oder einer Region, das/die zusätzliche altersbezogene Vorschriften (beispielsweise USA, Großbritannien, Europäische Union oder Südkorea) hat und das Alter des Benutzers befindet sich innerhalb der Spanne zwischen einem Minderjährigen und einem Erwachsenen (wie im entsprechenden Land oder der Region festgelegt). Im Allgemeinen, bedeutet dies, dass Teenager in regulierten Ländern als `notAdult` gelten.|
|minorNoParentalConsentRequired|5|Der Benutzer ist ein Miderjähriger, stammt jedoch aus einem Land oder einer Region, das/die keine altersbezogenen Vorschriften hat.|

#### <a name="age-group-and-minor-consent"></a>Altersgruppe und Zustimmung für den Minderjährigen

Die Altersgruppe und Zustimmung des Minderjährigen sind optionale Eigenschaften, die von Azure AD-Administratoren verwendet werden, um sicherzustellen, dass die Verwendung eines Kontos basierend auf den altersbezogenen behördlichen Vorschriften des Landes oder der Region des Benutzers ordnungsgemäß behandelt wird.

#### <a name="agegroup-property"></a>AgeGroup-Eigenschaft

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|keine|0|Standardwert nicht `ageGroup` wurde für den Benutzer festgelegt.|
|Minderjähriger|1|Der Benutzer ist als Minderjähriger zu berücksichtigen.|
|notAdult|2|Der Benutzer stammt aus einem Land, das gesetzliche Vorschriften hat, USA, Großbritannien, Europäische Union oder Südkorea) und das Alter des Benutzers liegt über der Obergrenze des Kindesalters (nach Land) und unter der Untergrenze für das Erwachsenenalter (festgelegt je nach Land oder Region). Teenager gelten in regulierten Länder als praktisch als `notAdult` .|
|Erwachsener|3|Der Benutzer sollte als Erwachsener behandelt werden..|

#### <a name="consentprovidedforminor-property"></a>ConsentProvidedForMinor-Eigenschaft

| Wert    | #  |Beschreibung|
|:---------------|:--------|:----------|
|keine|0|Standardwert nicht `consentProvidedForMinor` wurde für den Benutzer festgelegt.|
|gewährt|1|Für das Konto des Benutzers wurde eine Zustimmung eingeholt.|
|abgelehnt|2|Die Zustimmung zum Konto des Benutzers wurde nicht erteilt.|
|notRequired|3|Der Benutzer hat einen Standort, an dem eine Zustimmung nicht erforderlich ist.|
 
## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Aktivitäten|[UserActivity](projectrome_activity.md) -Sammlung|Die geräteübergreifenden Aktivitäten des Benutzers. Schreibgeschützt. Lässt Nullwerte zu.|
|Kalender|[Kalender](calendar.md)|Primärer Kalender des Benutzers. Schreibgeschützt.|
|calendarGroups|[CalendarGroup](calendargroup.md)-Sammlung|Die Kalendergruppen des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|calendarView|[Ereignis](event.md)-Sammlung|Die Kalenderansicht für den Kalender. Schreibgeschützt. Lässt NULL-Werte zu.|
|Kalender|[Kalendersammlung](calendar.md)|Die Kalender des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|contactFolders|[ContactFolder](contactfolder.md)-Sammlung|Die Kontakteordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|Kontakte|[Kontakte](contact.md)-Sammlung|Die Kontakte des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|createdObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die vom Benutzer erstellt wurden. Schreibgeschützt. Lässt NULL-Werte zu.|
|directReports|[directoryObject](directoryobject.md)-Sammlung|Die Benutzer und Kontakte, die an den Benutzer berichten. (Die Benutzer und Kontakte, deren manager-Eigenschaft auf diesen Benutzer festgelegt ist.) Schreibgeschützt. Lässt NULL-Werte zu. |
|Laufwerk|[Laufwerk](drive.md)|OneDrive eines Benutzers. Schreibgeschützt.|
|Laufwerke||||UNTRANSLATED_CONTENT_START|||[drive](drive.md) collection|||UNTRANSLATED_CONTENT_END|||| Eine Sammlung von Laufwerken, die für diesen Benutzer zur Verfügung stehen. Schreibgeschützt. |
|Ereignisse|[Ereignis](event.md)-Sammlung|Die Ereignisse des Benutzers. Standardmäßig werden Ereignisse unter dem Standard-Kalender angezeigt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für den Benutzer definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | Relevanzklassifizierung von Nachrichten des Benutzers basierend auf expliziten Kennzeichnungen, die die abgeleitete Relevanz oder Wichtigkeit außer Kraft setzen. |
|licenseDetails|[licenseDetails](licensedetails.md)-Sammlung|Eine Auflistung von Lizenzdetails des Benutzers. Lässt Nullwerte zu.|
|mailFolders|[MailFolder](mailfolder.md)-Sammlung| Die E-Mail-Ordner des Benutzers. Schreibgeschützt. Lässt NULL-Werte zu.|
|Verwalter|[directoryObject](directoryobject.md)|Der Benutzer oder Kontakt, der Vorgesetzter dieses Benutzers ist. Schreibgeschützt. (HTTP-Methoden: GET, PUT, DELETE.)|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Die Gruppen und Verzeichnisrollen, bei denen der Benutzer Mitglied ist. Schreibgeschützt. Lässt NULL-Werte zu.|
|Nachrichten|[Nachrichten](message.md)-Sammlung|Die Nachrichten in einem Postfach oder Ordner. Schreibgeschützt. Lässt NULL-Werte zu.|
|OneNote|[OneNote](onenote.md)| Schreibgeschützt.|
|Outlook|[OutlookUser](outlookuser.md)| Schreibgeschützt.|
|ownedDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|ownedObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die der Benutzer besitzt. Schreibgeschützt. Lässt NULL-Werte zu.|
|Personen|[Person](person.md)-Sammlung| Personen, die für den Benutzer relevant sind. Schreibgeschützt. Lässt Nullwerte zu.
|Foto|[profilePhoto](profilephoto.md)| Das Profilfoto des Benutzers. Schreibgeschützt.|
|Planner|[plannerUser](planneruser.md)| Einstiegspunkt für die Planner-Ressource, die für einen Benutzer vorhanden sein kann. Schreibgeschützt.|
|registeredDevices|[directoryObject](directoryobject.md)-Sammlung|Geräte, die für den Benutzer registriert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
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
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>Siehe auch

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
